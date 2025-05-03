---
layout: page
title: Natural Language Processing
description: NLP
img: assets/img/nlp_banner.png
importance: 1
category: lectures
related_publications: true
---

{% include figure.liquid loading="eager" path="assets/img/nlp_banner.png" title="Natural Language Processing" class="img-fluid rounded z-depth-1" %}
---

## 📋 Course Overview

| **Instructor:** | Edwin Puertas, PhD. | **Email:** | epuerta@utb.edu.co |
|:----------------|:-------------------|:-----------|:-------------------|
| **Office:** | AL-304 | **School:** | School of Digital Transformation |
| **Hours:** | 3 hours per week | **Credits:** | 4 |
| **Modality:** | Face-to-face | **Methodology:** | Lectures - Theoretical |

---

## 🎯 Course Purpose

> **Develop theoretical and practical competencies in Natural Language Processing (NLP)**, enabling students to apply machine learning techniques and models to analyze, understand, and generate text in various contexts, fostering the resolution of organizational and research problems with an ethical and sustainable approach.

### Specific Objectives

- 🧠 **Understand the theoretical foundations** of NLP, including language modeling, sentiment analysis, vector semantics, and neural networks
- 💻 **Implement supervised and unsupervised learning models** using Python, NLTK, and TensorFlow
- 📊 **Evaluate and optimize NLP models** through appropriate metrics and hyperparameter adjustments
- 👥 **Develop NLP projects in teams**, applying communication skills, collaboration, and critical thinking

---

## 🔄 Course Methodology

The learning process is supported by four main activities:

{% include course_methodology.html %}

<div class="methodology-grid">
  <div class="methodology-card">
    <h3>📝 Thematic Presentations</h3>
    <p>Synthesis of topics presented by the professor, enriched with valuable contributions and insights.</p>
  </div>
  <div class="methodology-card">
    <h3>👤 Student Assignments</h3>
    <p>Individual activities validating students' understanding and preparation of course materials.</p>
  </div>
  <div class="methodology-card">
    <h3>👥 Workshops</h3>
    <p>Group activities reinforcing learning through practical application of concepts and techniques.</p>
  </div>
  <div class="methodology-card">
    <h3>📋 Exams</h3>
    <p>Individual evaluations measuring learning progress throughout the course.</p>
  </div>
</div>

---

## 📚 Course Content

<div class="course-content">
  <table>
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

## 🔍 What is NLP?

<div class="nlp-definition">
  <p><strong>Natural Language Processing (NLP)</strong>, or Computational Linguistics, is concerned with theoretical and practical issues in the design and implementation of computer systems for processing human languages.</p>
</div>

---

## 🧩 NLP Fundamentals

### Language Processing Levels

<div class="language-levels">
  <div class="level-card">
    <h4>📢 Phonetics</h4>
    <p>The study of speech sounds, examining how sounds are produced, transmitted, and perceived</p>
  </div>
  <div class="level-card">
    <h4>🔊 Phonology</h4>
    <p>The study of sound systems and how sounds function within a particular language</p>
  </div>
  <div class="level-card">
    <h4>📝 Morphology</h4>
    <p>The study of word formation, examining morphemes (smallest meaningful units of language)</p>
  </div>
  <div class="level-card">
    <h4>🔄 Syntax</h4>
    <p>The study of sentence structure and arrangement of words and phrases</p>
  </div>
  <div class="level-card">
    <h4>💭 Semantics</h4>
    <p>The study of meaning in words and sentences, including lexical and compositional semantics</p>
  </div>
  <div class="level-card">
    <h4>👥 Pragmatics</h4>
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
  <div class="techniques-section">
    <h4>Techniques</h4>
    <ul>
      <li><strong>Tokenization:</strong> Dividing text into smaller units</li>
      <li><strong>Lemmatization/Stemming:</strong> Reducing words to base form</li>
      <li><strong>POS Tagging:</strong> Identifying grammatical functions</li>
      <li><strong>Dependency Parsing:</strong> Understanding syntactic relationships</li>
    </ul>
  </div>
  <div class="techniques-section">
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
  <div class="application-card">
    <h3>😃 Sentiment Analysis</h3>
    <p>Determining opinions or emotions expressed in text</p>
  </div>
  
  <div class="application-card">
    <h3>🤖 Chatbots</h3>
    <p>Automated conversations with users</p>
  </div>
  
  <div class="application-card">
    <h3>🌐 Machine Translation</h3>
    <p>Translating text between languages</p>
  </div>
  
  <div class="application-card">
    <h3>🔍 Information Extraction</h3>
    <p>Identifying and extracting relevant data from large text corpora</p>
  </div>
  
  <div class="application-card">
    <h3>✍️ Text Generation</h3>
    <p>Automatically creating original text</p>
  </div>
</div>

<!-- CSS for theme compatibility -->
<style>
  /* Base Styles with variables for theme compatibility */
  :root {
    --primary-color: #3a7bd5;
    --secondary-color: #00d2ff;
    --accent-color: #6d48e5;
    --text-color: #333;
    --text-color-light: #666;
    --background-color: #fff;
    --card-background: #f5f7fa;
    --border-color: #ddd;
    --hover-color: #f0f0f0;
    --table-header-bg: #3a7bd5;
    --table-header-text: #fff;
    --table-odd-row: #f7f7f7;
  }

  /* Dark theme overrides */
  @media (prefers-color-scheme: dark) {
    :root {
      --primary-color: #5c8eff;
      --secondary-color: #41c7ff;
      --accent-color: #9b7eff;
      --text-color: #e0e0e0;
      --text-color-light: #b0b0b0;
      --background-color: #1a1a1a;
      --card-background: #2a2a2a;
      --border-color: #444;
      --hover-color: #333;
      --table-header-bg: #2c5aa0;
      --table-header-text: #fff;
      --table-odd-row: #252525;
    }
  }

  /* General styling */
  body {
    color: var(--text-color);
    background-color: var(--background-color);
    font-family: -apple-system, BlinkMacSystemFont, "Segoe UI", Roboto, Helvetica, Arial, sans-serif;
    line-height: 1.6;
  }

  h1, h2, h3, h4 {
    color: var(--primary-color);
  }

  hr {
    border: 0;
    height: 1px;
    background: var(--border-color);
    margin: 2rem 0;
  }

  a {
    color: var(--primary-color);
    text-decoration: none;
  }

  a:hover {
    text-decoration: underline;
  }

  blockquote {
    border-left: 4px solid var(--primary-color);
    padding-left: 1rem;
    margin-left: 0;
    color: var(--text-color-light);
  }

  /* Tables */
  table {
    width: 100%;
    border-collapse: collapse;
    margin: 1rem 0;
    overflow: hidden;
    border-radius: 8px;
  }

  th {
    background-color: var(--table-header-bg);
    color: var(--table-header-text);
    padding: 0.75rem;
    text-align: left;
  }

  td {
    padding: 0.75rem;
    border: 1px solid var(--border-color);
  }

  tr:nth-child(odd) {
    background-color: var(--table-odd-row);
  }

  /* Course Methodology Grid */
  .methodology-grid {
    display: grid;
    grid-template-columns: repeat(auto-fit, minmax(250px, 1fr));
    gap: 1rem;
  }

  .methodology-card {
    background-color: var(--card-background);
    padding: 1rem;
    border-radius: 8px;
    border: 1px solid var(--border-color);
  }

  /* Course Content */
  .course-content table th {
    text-align: center;
  }

  .course-content ol {
    padding-left: 1.5rem;
    margin: 0;
  }

  /* Bibliography */
  .bibliography {
    background-color: var(--card-background);
    padding: 1rem;
    border-radius: 8px;
    border: 1px solid var(--border-color);
  }

  /* NLP Definition */
  .nlp-definition {
    background-color: var(--card-background);
    padding: 1rem;
    border-radius: 8px;
    border-left: 4px solid var(--primary-color);
  }

  /* Language Levels */
  .language-levels {
    display: grid;
    grid-template-columns: repeat(auto-fit, minmax(250px, 1fr));
    gap: 1rem;
  }

  .level-card {
    background-color: var(--card-background);
    padding: 1rem;
    border-radius: 8px;
    border: 1px solid var(--border-color);
  }

  /* Components Table */
  .components-table th {
    width: 30%;
  }

  /* Techniques Container */
  .techniques-container {
    display: grid;
    grid-template-columns: 1fr 1fr;
    gap: 1rem;
  }

  @media (max-width: 768px) {
    .techniques-container {
      grid-template-columns: 1fr;
    }
  }

  .techniques-section {
    background-color: var(--card-background);
    padding: 1rem;
    border-radius: 8px;
    border: 1px solid var(--border-color);
  }

  /* Applications Grid */
  .applications-grid {
    display: grid;
    grid-template-columns: repeat(auto-fit, minmax(200px, 1fr));
    gap: 1rem;
  }

  .application-card {
    background-color: var(--card-background);
    padding: 1rem;
    border-radius: 8px;
    text-align: center;
    border: 1px solid var(--border-color);
    transition: transform 0.2s;
  }

  .application-card:hover {
    transform: translateY(-5px);
  }
</style>
