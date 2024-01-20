<h1>Training a Sequence Classifier with PyTorch</h1>

<p>In this example, we demonstrate how to train a sequence classifier using PyTorch and the Hugging Face Transformers library. We'll use the MRPC (Microsoft Research Paraphrase Corpus) dataset as our example.</p>

<h2>Load and Process Data</h2>

<p>To load the MRPC dataset, we utilize the 🤗 Datasets library. The dataset contains pairs of sentences with labels indicating whether they are paraphrases or not.</p>

<code>
<pre>
from datasets import load_dataset
raw_datasets = load_dataset("glue", "mrpc")
</pre>
</code>

<p>The dataset is split into training, validation, and test sets, each with columns like 'sentence1', 'sentence2', 'label', and 'idx'.</p>

<h2>Preprocess Data</h2>

<p>We preprocess the dataset by tokenizing the sentences using a BERT-based tokenizer and converting them to a format suitable for the model.</p>

<code>
<pre>
from transformers import AutoTokenizer
tokenizer = AutoTokenizer.from_pretrained("bert-base-uncased")
# Tokenize dataset
tokenized_datasets = raw_datasets.map(tokenize_function, batched=True)
</pre>
</code>

<h2>Dynamic Padding</h2>

<p>To handle variable-length sequences, we dynamically pad the batches using the DataCollatorWithPadding provided by the Transformers library.</p>

<code>
<pre>
from transformers import DataCollatorWithPadding
data_collator = DataCollatorWithPadding(tokenizer=tokenizer)
# Example: Dynamic padding for a batch
samples = tokenized_datasets["train"][:8]
samples = {k: v for k, v in samples.items() if k not in ["idx", "sentence1", "sentence2"]}
batch = data_collator(samples)
</pre>
</code>

<p>Now, the data is ready for fine-tuning a sequence classification model!</p>
