# Hugging Face NLP Transformer
<hr>
<br>

<h1>Table of Content:</h1>
<table>
    <thead>
        <tr>
            <th><h3>S. No.</h3></th>
            <th><h3>Topic</h3></th>
            <th><h3>Content Covered</h3></th>
        </tr>
    </thead>
    <tbody>
        <tr>
            <td><h4>1</h4></td>
            <td><h5><span class="emoji">🔗</span><a href="https://github.com/UTSAVS26/Hugging-Face-NLP-Transformer/tree/main/Transformer%20Models">Day 01: Transformer Models</a></h5></td>
            <td>
                <ul>
                    <li><h5>Pipelines and Text Transformation</h5></li>
                    <li><h5>Transformer Architectures</h5></li>
                    <li><h5>Biases and Limitations</h5></li>
                </ul>
            </td>
        </tr>
        <tr>
            <td><h5>2</h5></td>
            <td><h5><span class="emoji">🔗</span><a href="https://github.com/UTSAVS26/Hugging-Face-NLP-Transformer/tree/main/Using%20Transformers">Day 02: Transformer Models and Tokenization</a></h5></td>
            <td>
                <ul>
                    <li><h5>Behind the Pipeline</h5></li>
                    <li><h5>Tokenizers</h5></li>
                    <li><h5>Handling Multiple Sequences</h5></li>
                    <li><h5>Models</h5></li>
                    <li><h5>Putting it All Together</h5></li>
                </ul>
            </td>
        </tr>
        <tr>
            <td><h5>3</h5></td>
            <td><h5><span class = "emoji">🔗</span><a href="https://github.com/UTSAVS26/Hugging-Face-NLP-Transformer/tree/main/Fine-Tuning%20a%20Pretrained%20Model">Day 03: Fine-Tuning a Pretrained Model</h5></td>
            <td>
                <ul>
                    <li><h5>Processing the Data</h5></li>
                    <li><h5>TFIne Tuning a Model with the Trainer API</h5></li>
                    <li><h5>A Full Training</h5></li>
                </ul>
            </td>
        </tr>
    </tbody>
</table>

<hr>

<h1><span class = "emoji">🔗</span><a href = "https://github.com/UTSAVS26/Hugging-Face-NLP-Transformer/tree/main/Transformer%20Models">Day 01: Transformer Models</a></h1>

<h2>Chapter 1. Unveiling the Power of Transformers <span class="emoji">🌟</span></h2>
<p>My journey began by exploring the transformative power of Transformer architectures—a groundbreaking paradigm shift in Natural Language Processing (NLP). The focal point was Hugging Face, a powerful library that has become a cornerstone in the realm of NLP. It opened doors to a Model Hub, featuring a rich collection of pretrained models designed to handle a diverse spectrum of language challenges.</p>

<h2>Chapter 2. Pipelines and Text Transformation <span class="emoji">🎭</span></h2>
<p>The highlight of the day was the discovery of Pipelines—a versatile tool that simplifies text transformation. This magic wand enabled seamless tasks, including sentiment analysis and text generation. It was a glimpse into the ease with which these models can manipulate and transform text.</p>

<h2>Chapter 3. Deciphering Transformer Architectures <span class="emoji">🧠📚</span></h2>
<p>Delving deeper into the intricacies, I explored the core of Transformer models. Encoders unravel language nuances, Decoders generate creative narratives, and the versatility of Encoder-Decoder models for tasks like summarization and translation left a lasting impression. Each layer revealed a new facet of the linguistic universe.</p>

<h2>Chapter 4. A Note on Biases <span class="emoji">⚠️</span></h2>
<p>Amidst the excitement, a crucial realization surfaced. Pretrained models, sourced from diverse internet data, inherently carried biases. An awareness of these biases became a key consideration, emphasizing the ethical use of these powerful tools. It's important to note that pretrained models may carry biases, necessitating careful consideration for their ethical use.</p>

<hr>

<h1><span class = "emoji">🔗</span><a href="https://github.com/UTSAVS26/Hugging-Face-NLP-Transformer/tree/main/Using%20Transformers">Day 02: Transformer Models and Tokenization</a></h1>

<h2>Chapter 1. Tokenization Pipeline</h2>
<p>Learned about the components of the NLP tokenization pipeline and its importance in translating text into numerical data.</p>

<h2>Chapter 2. Different Tokenization Techniques</h2>
<table>
    <tbody>
        <tr>
            <td><h4>Word-based Tokenization</h4></td>
            <td>Explored word-based tokenization, where text is split into words to create a numerical representation for each word.</td>
        </tr>
        <tr>
            <td><h4>Character-based Tokenization</h4></td>
            <td>Introduced character-based tokenization as an alternative, which splits text into characters, resulting in a smaller vocabulary.</td>
        </tr>
        <tr>
            <td><h4>Subword Tokenization</h4></td>
            <td>Discussed subword tokenization algorithms, combining the benefits of both word-based and character-based approaches.</td>
        </tr>
    </tbody>
</table>

<h2>Chapter 3. Loading and Saving Tokenizers</h2>
<p>Learned how to load and save tokenizers, crucial for maintaining consistency between training and inference.</p>

<h2>Chapter 4. Encoding and Decoding</h2>
<p>Explored the encoding process, translating text into numbers, and decoding, converting vocabulary indices back to a string.</p>

<h2>Chapter 6. Handling Multiple Sequences</h2>
<p>Addressed challenges related to handling multiple sequences, different sequence lengths, and introduced batching, padding, and attention masks.</p>

<h2>Chapter 7. Putting it All Together</h2>
<p>Understood how the 🤗 Transformers API simplifies the entire process, from tokenization to model input, handling various scenarios.</p>

<h2>Conclusion</h2>
<p>Recapped the key takeaways, enabling the navigation of 🤗 Transformers documentation with a familiar understanding of concepts.</p>

<hr>

<h1><span class = "emoji">🔗</span><a href="https://github.com/UTSAVS26/Hugging-Face-NLP-Transformer/tree/main/Fine-Tuning%20a%20Pretrained%20Model">Day 03: Fine-Tuning a Pretrained Model</h1>

<h2>Overview</h2>
<ul>
  <li>Introduction to fine-tuning for adapting pretrained models.</li>
  <li>Leveraging pretrained knowledge for downstream tasks.</li>
</ul>

<h2>Chapter 1: Data Preprocessing</h2>
<ul>
  <li>Loading GLUE MRPC dataset for fine-tuning.</li>
  <li>Selection of pretrained model checkpoint.</li>
</ul>

<h2>Chapter 2: Tokenization and Dataset Preparation</h2>
<ul>
  <li>Tokenization using AutoTokenizer for compatibility.</li>
  <li>DataCollatorWithPadding implementation for handling input length variations.</li>
</ul>

<h2>Chapter 3: Training Configuration</h2>
<ul>
  <li>Utilization of TrainingArguments for hyperparameter settings.</li>
  <li>Specifying the directory for saving the trained model.</li>
</ul>

<h2>Chapter 4: Model Configuration</h2>
<ul>
  <li>Use of AutoModelForSequenceClassification for defining the model architecture.</li>
  <li>Warnings about model head modification and implications for sequence classification.</li>
</ul>

<h2>Chapter 5: Trainer Configuration</h2>
<ul>
  <li>Configuration of the Trainer class, incorporating model, training arguments, datasets, and collators.</li>
  <li>Emphasis on GPU usage due to computational demands.</li>
</ul>

<h2>Chapter 6: Evaluation</h2>
<ul>
  <li>Importance of evaluating the model's performance during training.</li>
  <li>Introduction to compute_metrics using the 🤗 Evaluate library for metrics calculation.</li>
</ul>

<h2>Chapter 7: Accelerated Training with 🤗 Accelerate</h2>
<ul>
  <li>Overview of 🤗 Accelerate for simplifying distributed training.</li>
  <li>Adjustments to the training loop and optimizer for harnessing 🤗 Accelerate's capabilities.</li>
</ul>
