---
layout: page
title: Natural Language Processing
description: 
img: assets/img/nlp_banner.png
importance: 1
category: courses
related_publications: true
---

{% include figure.liquid loading="eager" path="assets/img/nlp_banner.png" title="Natural Language Processing" class="img-fluid rounded z-depth-1" %}
---

## 📋 Course Overview

<table>
  <thead>
    <tr>
      <th colspan="4">Course Information</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td><strong>Instructor:</strong></td>
      <td>Edwin Puertas, PhD.</td>
      <td><strong>Email:</strong></td>
      <td>epuerta@utb.edu.co</td>
    </tr>
    <tr>
      <td><strong>Office:</strong></td>
      <td>AL-304</td>
      <td><strong>School:</strong></td>
      <td>School of Digital Transformation</td>
    </tr>
    <tr>
      <td><strong>Hours:</strong></td>
      <td>3 hours per week</td>
      <td><strong>Credits:</strong></td>
      <td>4</td>
    </tr>
    <tr>
      <td><strong>Modality:</strong></td>
      <td>Face-to-face</td>
      <td><strong>Methodology:</strong></td>
      <td>Lectures - Theoretical</td>
    </tr>
  </tbody>
</table>

---

## 🎯 Course Purpose

> **Develop theoretical and practical competencies in Natural Language Processing (NLP)**, enabling students to apply machine learning techniques and models to analyze, understand, and generate text in various contexts, fostering the resolution of organizational and research problems with an ethical and sustainable approach.

### Specific Objectives

- **Understand the theoretical foundations** of NLP, including language modeling, sentiment analysis, vector semantics, and neural networks
- **Implement supervised and unsupervised learning models** using Python, NLTK, and TensorFlow
- **Evaluate and optimize NLP models** through appropriate metrics and hyperparameter adjustments
- **Develop NLP projects in teams**, applying communication skills, collaboration, and critical thinking

---

## 📚 Course Content

<table class="module-table">
  <thead>
    <tr>
      <th>Module 1:<br>Fundamentals of NLP</th>
      <th>Module 2:<br>Machine Learning & NLP</th>
      <th>Module 3:<br>Applications and Ethics</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td>
        <ol>
          <li>Introduction to NLP and human language technologies</li>
          <li>Regular expressions, text normalization, and edit distance</li>
          <li>Language modeling with N-Grams</li>
          <li>Text classification with Naïve Bayes and sentiment analysis</li>
          <li>Logistic regression and vector semantics</li>
        </ol>
      </td>
      <td>
        <ol>
          <li>Neural networks and neural language models</li>
          <li>Sequence labeling for parts of speech and named entities</li>
          <li>RNNs, LSTMs, and advanced language models</li>
          <li>Transformers and large language models (BERT, GPT)</li>
          <li>Fine-tuning, prompting, and in-context learning</li>
        </ol>
      </td>
      <td>
        <ol>
          <li>Machine translation and text generation</li>
          <li>Question answering and information retrieval</li>
          <li>Development of chatbots and dialogue systems</li>
          <li>Automatic speech recognition and voice synthesis</li>
          <li>Ethical considerations in NLP and applications in reducing inequalities</li>
        </ol>
      </td>
    </tr>
  </tbody>
</table>

---

## 🔄 Course Methodology

The learning process is supported by four main activities:

<div class="methodology-grid">
  <div class="methodology-item">
    <h3>📝 Thematic Presentations</h3>
    <p>Synthesis of topics presented by the professor, enriched with valuable contributions and insights.</p>
  </div>
  <div class="methodology-item">
    <h3>👤 Student Assignments</h3>
    <p>Individual activities validating students' understanding and preparation of course materials.</p>
  </div>
  <div class="methodology-item">
    <h3>👥 Workshops</h3>
    <p>Group activities reinforcing learning through practical application of concepts and techniques.</p>
  </div>
  <div class="methodology-item">
    <h3>📋 Exams</h3>
    <p>Individual evaluations measuring learning progress throughout the course.</p>
  </div>
</div>

---

## 🔍 What is NLP?

<div class="definition-box">
  <p><strong>Natural Language Processing (NLP)</strong>, or Computational Linguistics, is concerned with theoretical and practical issues in the design and implementation of computer systems for processing human languages.</p>
</div>

---

## 🧩 NLP Fundamentals

### Language Processing Levels

<div class="levels-grid">
  <div class="level-item">
    <h4>Phonetics</h4>
    <p>The study of speech sounds, examining how sounds are produced, transmitted, and perceived</p>
  </div>
  <div class="level-item">
    <h4>Phonology</h4>
    <p>The study of sound systems and how sounds function within a particular language</p>
  </div>
  <div class="level-item">
    <h4>Morphology</h4>
    <p>The study of word formation, examining morphemes (smallest meaningful units of language)</p>
  </div>
  <div class="level-item">
    <h4>Syntax</h4>
    <p>The study of sentence structure and arrangement of words and phrases</p>
  </div>
  <div class="level-item">
    <h4>Semantics</h4>
    <p>The study of meaning in words and sentences, including lexical and compositional semantics</p>
  </div>
  <div class="level-item">
    <h4>Pragmatics</h4>
    <p>The study of language use in social contexts, considering factors like speaker intention and implied meaning</p>
  </div>
</div>

### Key NLP Components

<table class="components-table">
  <thead>
    <tr>
      <th>Component</th>
      <th>Description</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td><strong>Text Preprocessing</strong></td>
      <td>Preparing raw text for analysis by transforming it into machine-readable format</td>
    </tr>
    <tr>
      <td><strong>Feature Extraction</strong></td>
      <td>Converting raw text into numerical representations</td>
    </tr>
    <tr>
      <td><strong>POS Tagging</strong></td>
      <td>Identifying the grammatical function of each word</td>
    </tr>
    <tr>
      <td><strong>Named Entity Recognition</strong></td>
      <td>Identifying useful entities like names, locations, and dates</td>
    </tr>
    <tr>
      <td><strong>Coreference Resolution</strong></td>
      <td>Identifying when different words refer to the same entity</td>
    </tr>
    <tr>
      <td><strong>Parsing</strong></td>
      <td>Analyzing grammatical structure to extract meaning</td>
    </tr>
  </tbody>
</table>

### Fundamental Techniques & Algorithms

<div class="techniques-container">
  <div class="techniques-column">
    <h4>Techniques</h4>
    <ul>
      <li><strong>Tokenization:</strong> Dividing text into smaller units</li>
      <li><strong>Lemmatization/Stemming:</strong> Reducing words to base form</li>
      <li><strong>POS Tagging:</strong> Identifying grammatical functions</li>
      <li><strong>Dependency Parsing:</strong> Understanding syntactic relationships</li>
    </ul>
  </div>
  <div class="techniques-column">
    <h4>Algorithms</h4>
    <ul>
      <li><strong>Bag of Words:</strong> Simple representation of word frequency</li>
      <li><strong>TF-IDF:</strong> Weighting word importance in documents</li>
      <li><strong>Word Embeddings:</strong> Vector representations of words</li>
      <li><strong>N-gram Models:</strong> Predicting words based on context</li>
      <li><strong>Pre-trained Models:</strong> Models trained on massive text corpora</li>
    </ul>
  </div>
</div>

---

## 🚀 Practical Applications of NLP

<div class="applications-grid">
  <div class="application-item">
    <h3>😃 Sentiment Analysis</h3>
    <p>Determining opinions or emotions expressed in text</p>
  </div>
  
  <div class="application-item">
    <h3>🤖 Chatbots</h3>
    <p>Automated conversations with users</p>
  </div>
  
  <div class="application-item">
    <h3>🌐 Machine Translation</h3>
    <p>Translating text between languages</p>
  </div>
  
  <div class="application-item">
    <h3>🔍 Information Extraction</h3>
    <p>Identifying and extracting relevant data from large text corpora</p>
  </div>
  
  <div class="application-item">
    <h3>✍️ Text Generation</h3>
    <p>Automatically creating original text</p>
  </div>
</div>

---

## 📖 Bibliography

<div class="bibliography">
  <ul>
    <li>Dan Jurafsky and James H. Martin (2020), <em>Speech and Language Processing</em> (3rd ed. draft)</li>
    <li>Beysolow II, T. (2018). <em>Applied Natural Language Processing with Python: Implementing Machine Learning and Deep Learning Algorithms for Natural Language Processing</em>. Apress.</li>
    <li>Vajjala, S., Majumder, B., Gupta, A., & Surana, H. (2020). <em>Practical Natural Language Processing: A Comprehensive Guide to Building Real-World NLP Systems</em>. O'Reilly Media.</li>
    <li>Srinivasa-Desikan, B. (2018). <em>Natural Language Processing and Computational Linguistics: A practical guide to text analysis with Python, Gensim, spaCy, and Keras</em>. Packt Publishing Ltd.</li>
  </ul>
</div>

---


<!-- Add this CSS at the bottom of your Markdown file or in your theme's CSS file -->
<style>
/* Enhanced tables for better dark mode compatibility */
table {
  width: 100%;
  border-collapse: collapse;
  margin: 20px 0;
  border: 1px solid var(--table-border-color, #444);
}

table th {
  background-color: var(--table-header-bg, #333);
  color: var(--table-header-color, #fff);
  padding: 12px 15px;
  text-align: left;
  border: 1px solid var(--table-border-color, #444);
}

table td {
  padding: 12px 15px;
  border: 1px solid var(--table-border-color, #444);
  background-color: var(--table-cell-bg, rgba(255, 255, 255, 0.05));
}

table tr:nth-child(even) td {
  background-color: var(--table-cell-alt-bg, rgba(255, 255, 255, 0.02));
}

/* Grid layouts for methodology and applications */
.methodology-grid, .levels-grid, .applications-grid {
  display: grid;
  grid-template-columns: repeat(auto-fit, minmax(300px, 1fr));
  gap: 20px;
  margin-bottom: 20px;
}

.methodology-item, .level-item, .application-item {
  padding: 20px;
  border-radius: 8px;
  background-color: var(--card-bg, rgba(255, 255, 255, 0.05));
  border: 1px solid var(--card-border-color, #444);
}

/* Definition box styling */
.definition-box {
  padding: 20px;
  border-left: 5px solid var(--accent-color, #0066cc);
  margin: 20px 0;
  background-color: var(--definition-bg, rgba(255, 255, 255, 0.05));
}

/* Bibliography styling */
.bibliography {
  padding: 20px;
  background-color: var(--bibliography-bg, rgba(255, 255, 255, 0.03));
  border-radius: 8px;
}

/* Techniques container */
.techniques-container {
  display: grid;
  grid-template-columns: repeat(auto-fit, minmax(250px, 1fr));
  gap: 20px;
}

/* Module table styling */
.module-table th {
  text-align: center;
  vertical-align: middle;
}

.module-table td {
  vertical-align: top;
}

/* Components table styling */
.components-table td:first-child {
  width: 30%;
}

/* Dark mode specific overrides */
@media (prefers-color-scheme: dark) {
  :root {
    --table-border-color: #444;
    --table-header-bg: #222;
    --table-header-color: #fff;
    --table-cell-bg: rgba(255, 255, 255, 0.05);
    --table-cell-alt-bg: rgba(255, 255, 255, 0.02);
    --card-bg: rgba(255, 255, 255, 0.05);
    --card-border-color: #444;
    --accent-color: #3a7bd5;
    --definition-bg: rgba(255, 255, 255, 0.05);
    --bibliography-bg: rgba(255, 255, 255, 0.03);
  }
}
</style>
