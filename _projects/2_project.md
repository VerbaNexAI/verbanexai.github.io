---
layout: page
title: Early Detection of Depression and Anxiety
description: Multimodal System for Early Detection of Depression and Anxiety in University Population
img: assets/img/banner-thesis-jeison.jpg
importance: 2
category: Master's degree
giscus_comments: true
---

# 🧠 Multimodal System for Early Detection of Depression and Anxiety in University Population

---

## Context: The Silent Crisis in Higher Education

Mental health in the university setting represents one of the most urgent challenges in contemporary public health. Recent studies in Latin America reveal alarming prevalence rates exceeding 60% for depressive and anxiety symptoms among higher education students. In Colombia specifically, 35% of young people between 18 and 26 years old reported suicidal ideation during the pandemic, with a probability four times higher compared to older adults.

**The problem is aggravated** by the critical shortage of professional mental health resources, with only 3.5 psychiatrists per 100,000 inhabitants in the country, severely limiting access to timely specialized evaluations.

<div class="diagram-container">
  <div class="crisis-diagram">
    <div class="node main-node">Mental Health Crisis<br>in University Students</div>
    <div class="connector"></div>
    <div class="node-group">
      <div class="node">Latin America:<br>60-71% Prevalence</div>
      <div class="node">Colombia:<br>35% Suicidal Ideation</div>
      <div class="node">Critical Shortage:<br>3.5 Psychiatrists/100k inhab</div>
    </div>
    <div class="connector"></div>
    <div class="node secondary-node">Limitations of<br>Traditional Detection</div>
    <div class="connector"></div>
    <div class="node-group">
      <div class="node">Subjectivity</div>
      <div class="node">Limited Scalability</div>
      <div class="node">Discontinuous Monitoring</div>
    </div>
  </div>
</div>
---
## Our Proposal: Integrated Multimodal Approach

Faced with these limitations, we developed an artificial intelligence system that integrates simultaneous analysis of text, audio, and video for early detection of depression and anxiety indicators. The fundamental premise is that mental health disorders manifest heterogeneously through multiple behavioral channels, and multimodal integration allows capturing this complexity more comprehensively.

**Scientific evidence** supports this approach: recent studies demonstrate improvements of up to 25% in accuracy metrics when integrating multiple modalities compared to unimodal systems. This is because different modalities capture complementary aspects of symptomatic manifestations.

<div class="diagram-container">
  <div class="multimodal-flow">
    <div class="flow-row">
      <div class="modality-node">
        <div class="modality-icon">📝</div>
        <div class="modality-text">Text<br>Semantic Analysis</div>
      </div>
      <div class="modality-node">
        <div class="modality-icon">🎵</div>
        <div class="modality-text">Audio<br>Acoustic Features</div>
      </div>
      <div class="modality-node">
        <div class="modality-icon">📹</div>
        <div class="modality-text">Video<br>Facial Expressions</div>
      </div>
    </div>
    <div class="flow-arrow">↓</div>
    <div class="fusion-node">
      <div class="fusion-text">Multimodal Fusion</div>
    </div>
    <div class="flow-arrow">↓</div>
    <div class="result-node">
      <div class="result-text">Indicator Detector → Results Prioritization</div>
    </div>
  </div>
</div>
---
### Scientific Foundations by Modality

**Text Analysis:** Examines linguistic patterns characteristic of depressive and anxious states, including predominantly negative vocabulary, persistent self-critical expressions, and ruminative thinking patterns. We use Spanish BERT models fine-tuned for clinical-educational context.

**Audio Processing:** Captures paralinguistic characteristics such as monotonous voice, prolonged pauses, reduced tonal variation, and decreased speech rate. We implement advanced acoustic feature extractors like MFCC and eGeMAPS combined with pre-trained models like Wav2Vec 2.0.

**Visual Analysis:** Detects changes in facial expressions through tracking of Facial Action Units (FAUs), reduced frequency of genuine smiles, empty or furrowed expressions, and gaze patterns. We employ OpenFace for robust extraction of visual biomarkers.

## System Architecture

The system follows a modular architecture that allows independent processing of each modality before integration through advanced fusion mechanisms. This approach ensures that specific information from each channel is preserved while capturing inter-modal correlations.

**Integration Process:** Each modality is processed through specialized neural networks, whose representations are combined through multi-head attention mechanisms that dynamically learn the relative importance of each modality according to the specific context and individual student characteristics.

<div class="diagram-container">
  <div class="architecture-diagram">
    <div class="arch-node input-node">
      <div class="arch-title">Multimodal Input</div>
      <div class="arch-subtitle">Text + Audio + Video</div>
    </div>
    <div class="arch-arrow">↓</div>
    <div class="arch-node process-node">
      <div class="arch-title">Feature Extraction</div>
    </div>
    <div class="arch-arrow">↓</div>
    <div class="arch-row">
      <div class="arch-module">
        <div class="module-title">Text Model</div>
        <div class="module-detail">Spanish BERT</div>
      </div>
      <div class="arch-module">
        <div class="module-title">Audio Model</div>
        <div class="module-detail">Wav2Vec 2.0 + MFCC</div>
      </div>
      <div class="arch-module">
        <div class="module-title">Video Model</div>
        <div class="module-detail">OpenFace + FAUs</div>
      </div>
    </div>
    <div class="arch-arrow">↓</div>
    <div class="arch-node fusion-node">
      <div class="arch-title">Fusion with Multi-head Attention</div>
    </div>
    <div class="arch-arrow">↓</div>
    <div class="arch-node classifier-node">
      <div class="arch-title">Classifier</div>
      <div class="arch-subtitle">Depression/Anxiety</div>
    </div>
    <div class="arch-arrow">↓</div>
    <div class="arch-node output-node">
      <div class="arch-title">Output</div>
      <div class="arch-subtitle">Indicators + Prioritization</div>
    </div>
  </div>
</div>
---
## Development Methodology

The project follows the **Design Science Research** methodology, an iterative approach that ensures systematic development of technological artifacts with practical applicability in specific domains. This methodology is structured in four main phases that guide the process from problem identification to final system validation.

**Key characteristic** of this approach is its iterative nature, allowing progressive refinement based on continuous empirical evaluation and expert feedback at each development stage.

<div class="diagram-container">
  <div class="methodology-diagram">
    <div class="phase phase-1">
      <div class="phase-number">1</div>
      <div class="phase-content">
        <div class="phase-title">Literature Review and Problem Definition</div>
      </div>
    </div>
    <div class="phase-arrow">↓</div>
    <div class="phase phase-2">
      <div class="phase-number">2</div>
      <div class="phase-content">
        <div class="phase-title">Ethical Protocol and Consent</div>
      </div>
    </div>
    <div class="phase-arrow">↓</div>
    <div class="phase-group">
      <div class="phase-sub">
        <div class="phase-sub-title">Participant Recruitment</div>
      </div>
      <div class="phase-sub">
        <div class="phase-sub-title">Multimodal Data Collection</div>
      </div>
      <div class="phase-sub">
        <div class="phase-sub-title">Labeling PHQ-9/GAD-7</div>
      </div>
    </div>
    <div class="phase-arrow">↓</div>
    <div class="phase phase-3">
      <div class="phase-number">3</div>
      <div class="phase-content">
        <div class="phase-title">Labeled Multimodal Corpus</div>
      </div>
    </div>
    <div class="phase-arrow">↓</div>
    <div class="phase-group">
      <div class="phase-sub">
        <div class="phase-sub-title">Model Training by Modality</div>
      </div>
      <div class="phase-sub">
        <div class="phase-sub-title">Fusion Strategies Development</div>
      </div>
      <div class="phase-sub">
        <div class="phase-sub-title">Hyperparameter Optimization</div>
      </div>
    </div>
    <div class="phase-arrow">↓</div>
    <div class="phase phase-4">
      <div class="phase-number">4</div>
      <div class="phase-content">
        <div class="phase-title">Integrated System API + Interface</div>
      </div>
    </div>
    <div class="phase-arrow">↓</div>
    <div class="phase phase-5">
      <div class="phase-number">5</div>
      <div class="phase-content">
        <div class="phase-title">Validation with Experts</div>
      </div>
    </div>
    <div class="phase-arrow">↓</div>
    <div class="phase phase-6">
      <div class="phase-number">6</div>
      <div class="phase-content">
        <div class="phase-title">Final Evaluation and Documentation</div>
      </div>
    </div>
  </div>
</div>

### Phase 1: Problem Identification

Comprises a systematic literature review on multimodal AI systems for depression and anxiety detection, using the ProKnow-C technique for structured selection and analysis of relevant bibliography.

### Phase 2: Objective Definition

Establishes the functional and non-functional requirements of the system, along with the detailed architectural design that considers aspects of modularity, maintainability, and adaptability for future extensions.

### Phase 3: Iterative Design and Development

Structured in four specialized iterations:
- **Iteration 1:** Ethical protocol and data processing
- **Iteration 2:** Multimodal corpus construction
- **Iteration 3:** Fusion model development
- **Iteration 4:** System integration and refinement

### Phase 4: Demonstration and Validation

Includes empirical evaluation with test data, comparative analysis with state-of-the-art methods, and usability testing with mental health professionals to validate practical applicability.

## Application in University Context

The system is specifically designed for university environments, considering the demographic, cultural, and logistical particularities of this population. The implementation is conceived as a first-line screening tool that complements, does not replace, specialized professional evaluation.

**Intervention flow:** Students interact with the system through brief sessions where they answer open questions while their responses are captured in text, audio, and video. The system analyzes these signals and generates a risk profile that allows intelligent case prioritization according to the severity of detected indicators.

<div class="diagram-container">
  <div class="intervention-flow">
    <div class="intervention-step">
      <div class="step-icon">👤</div>
      <div class="step-text">Student</div>
    </div>
    <div class="step-arrow">→</div>
    <div class="intervention-step">
      <div class="step-icon">🤖</div>
      <div class="step-text">Multimodal System</div>
    </div>
    <div class="step-arrow">→</div>
    <div class="intervention-step">
      <div class="step-icon">⚡</div>
      <div class="step-text">Real-time Analysis</div>
    </div>
    <div class="step-arrow">→</div>
    <div class="priority-group">
      <div class="priority-item mild">
        <div class="priority-title">Mild Indicators</div>
        <div class="priority-desc">Automated Monitoring</div>
      </div>
      <div class="priority-item moderate">
        <div class="priority-title">Moderate Indicators</div>
        <div class="priority-desc">Scheduled Referral</div>
      </div>
      <div class="priority-item severe">
        <div class="priority-title">Severe Indicators</div>
        <div class="priority-desc">Immediate Prioritization</div>
      </div>
    </div>
    <div class="step-arrow">→</div>
    <div class="intervention-step final">
      <div class="step-icon">📊</div>
      <div class="step-text">Resource Optimization<br>University Welfare</div>
    </div>
  </div>
</div>

**Initial target population:** Systems Engineering and Psychology students from Universidad Tecnológica de Bolívar, with potential for expansion to other faculties and institutions.

## Ethical and Privacy Considerations

The system development incorporates from its design fundamental ethical considerations to guarantee participant protection and responsible technology use.

**Modal informed consent:** We design specific consent forms for each data type (text, audio, video), recognizing that these modalities present different sensitivity levels and protection requirements.

**Robust anonymization:** We implement advanced anonymization techniques that guarantee protection of participant identity through elimination of personal identifiers and obfuscation of sensitive attributes.

**Algorithmic equity:** We incorporate mechanisms to mitigate demographic biases and ensure the system functions equitably across different population groups.

<div class="diagram-container">
  <div class="ethics-diagram">
    <div class="ethics-center">
      <div class="ethics-main">Participant Protection</div>
    </div>
    <div class="ethics-branches">
      <div class="ethics-branch">
        <div class="branch-line"></div>
        <div class="ethics-node">
          <div class="ethics-title">Informed Consent<br>by Modality</div>
        </div>
        <div class="branch-line"></div>
        <div class="ethics-leaf">
          <div class="leaf-text">Equity in Detection<br>Without Demographic Biases</div>
        </div>
      </div>
      <div class="ethics-branch">
        <div class="branch-line"></div>
        <div class="ethics-node">
          <div class="ethics-title">Anonymization of<br>Sensitive Data</div>
        </div>
        <div class="branch-line"></div>
        <div class="ethics-leaf">
          <div class="leaf-text">Privacy Preserved<br>Identity Protected</div>
        </div>
      </div>
      <div class="ethics-branch">
        <div class="branch-line"></div>
        <div class="ethics-node">
          <div class="ethics-title">Transparency in<br>Data Use</div>
        </div>
        <div class="branch-line"></div>
        <div class="ethics-leaf">
          <div class="leaf-text">Institutional and<br>Student Trust</div>
        </div>
      </div>
    </div>
  </div>
</div>

## Expected Products

The project will generate several tangible products that will benefit both the academic community and educational institutions:

<div class="table-container">
  <table class="products-table">
    <thead>
      <tr>
        <th>Product</th>
        <th>Description</th>
        <th>Impact</th>
      </tr>
    </thead>
    <tbody>
      <tr>
        <td><strong>Multimodal Ethical Protocol</strong></td>
        <td>Document with procedures for consensual multimodal data collection, including specific consent forms by modality and verifiable anonymization protocols.</td>
        <td>Establishes replicable standards for responsible research with sensitive data in educational environments.</td>
      </tr>
      <tr>
        <td><strong>Labeled Multimodal Corpus</strong></td>
        <td>Database with text, audio, and video samples from university students, synchronized and labeled with PHQ-9 and GAD-7 scales.</td>
        <td>First resource of its kind in Spanish for Colombian university context, facilitating future research.</td>
      </tr>
      <tr>
        <td><strong>Trained Fusion Architectures</strong></td>
        <td>Implemented and optimized AI models including early, intermediate, and late fusion systems, specifically trained for depression and anxiety detection.</td>
        <td>Advances state of the art in multimodal fusion techniques for mental health applications.</td>
      </tr>
      <tr>
        <td><strong>Integrated Detection System</strong></td>
        <td>Functional platform with API for real-time analysis, user interface for result visualization, and modular scalable architecture for institutional implementation.</td>
        <td>Practical tool that can be adopted by university welfare services to optimize their resources.</td>
      </tr>
    </tbody>
  </table>
</div>

## Research Team

**Principal Investigator:**  
Jeison David Jiménez Alvear - Master's in Engineering with Emphasis on Systems and Computing, Universidad Tecnológica de Bolívar. Research assistant with experience in natural language processing and machine learning.

**Directors:**  
- **Dr. Edwin Puertas:** Artificial Intelligence Software Architect and Researcher in Natural Language Processing, with 20 years of experience in academic and professional fields. Director of Doctoral and Master's Programs in Engineering at UTB.
- **Dr. Juan Carlos Martínez:** Electronic Engineer, Doctor from Northeastern University, Boston. Fulbright-DNP-Colciencias Fellow 2007. Researcher and professor at UTB since 2004.
- **Dr. Karol Gutiérrez:** Psychologist, Master in Neuropsychology and Doctor in Neuropsychology from University of Salamanca. Specialist in development of cognitive processes and neuroscience applied to education.

## Expected Impact

The successful development of this multimodal system has the potential to generate significant impacts in multiple dimensions:

**Impact on Student Health:** Earlier and more accurate detection of at-risk students, allowing timely interventions that can prevent symptom progression and reduce cases of unattended mental health crises.

**Academic Impact:** Potential reduction of academic dropout related to mental health problems, through identification and proactive support of students experiencing difficulties.

**Institutional Impact:** Optimization of limited university welfare resources through intelligent case prioritization, ensuring students with greatest need receive timely attention.

**Scientific Impact:** Advancement of state of the art in multimodal detection of mental health problems, particularly in Spanish-speaking contexts and educational environments.

**Social Impact:** Establishment of ethical and technical standards for responsible use of artificial intelligence in sensitive applications like mental health, creating precedents for similar future initiatives.

---

<style>
/* ============================================
   MULTIMODAL SYSTEM DIAGRAMS - IMPROVED STYLES
   Compatible with Al-Folio light/dark themes
   ============================================ */

:root {
  /* Light theme colors */
  --diagram-bg-light: #f8f9fa;
  --diagram-border-light: #e9ecef;
  --node-bg-light: #ffffff;
  --text-primary-light: #2d3748;
  --text-secondary-light: #4a5568;
  --primary-color-light: #007acc;
  --success-color-light: #28a745;
  --warning-color-light: #ffc107;
  --danger-color-light: #dc3545;
  --shadow-light: rgba(0, 0, 0, 0.1);
  
  /* Dark theme colors */
  --diagram-bg-dark: #1a202c;
  --diagram-border-dark: #2d3748;
  --node-bg-dark: #2d3748;
  --text-primary-dark: #e2e8f0;
  --text-secondary-dark: #cbd5e0;
  --primary-color-dark: #4299e1;
  --success-color-dark: #48bb78;
  --warning-color-dark: #ecc94b;
  --danger-color-dark: #f56565;
  --shadow-dark: rgba(0, 0, 0, 0.3);
}

/* Base diagram container */
.diagram-container {
  margin: 3rem 0;
  padding: 2rem;
  background: var(--diagram-bg-light);
  border-radius: 16px;
  border: 1px solid var(--diagram-border-light);
  transition: all 0.3s ease;
}

/* Dark theme support */
html[data-theme='dark'] .diagram-container,
.dark-mode .diagram-container,
[data-theme='dark'] .diagram-container {
  background: var(--diagram-bg-dark);
  border-color: var(--diagram-border-dark);
}

/* ============================================
   CRISIS DIAGRAM STYLES
   ============================================ */

.crisis-diagram {
  display: flex;
  flex-direction: column;
  align-items: center;
  gap: 1.5rem;
}

.node {
  background: var(--node-bg-light);
  border: 2px solid var(--primary-color-light);
  border-radius: 12px;
  padding: 1.25rem;
  margin: 0.5rem;
  text-align: center;
  box-shadow: 0 4px 12px var(--shadow-light);
  min-width: 200px;
  font-weight: 500;
  color: var(--text-primary-light);
  transition: all 0.3s ease;
}

html[data-theme='dark'] .node,
.dark-mode .node,
[data-theme='dark'] .node {
  background: var(--node-bg-dark);
  border-color: var(--primary-color-dark);
  color: var(--text-primary-dark);
  box-shadow: 0 4px 16px var(--shadow-dark);
}

.node:hover {
  transform: translateY(-2px);
  box-shadow: 0 6px 16px var(--shadow-light);
}

html[data-theme='dark'] .node:hover,
.dark-mode .node:hover,
[data-theme='dark'] .node:hover {
  box-shadow: 0 6px 20px var(--shadow-dark);
}

.main-node {
  background: linear-gradient(135deg, var(--primary-color-light), #0056b3);
  color: white;
  font-weight: bold;
  font-size: 1.15em;
  border-color: var(--primary-color-light);
}

html[data-theme='dark'] .main-node,
.dark-mode .main-node,
[data-theme='dark'] .main-node {
  background: linear-gradient(135deg, var(--primary-color-dark), #2c5282);
  border-color: var(--primary-color-dark);
}

.secondary-node {
  background: linear-gradient(135deg, var(--success-color-light), #1e7e34);
  color: white;
  border-color: var(--success-color-light);
}

html[data-theme='dark'] .secondary-node,
.dark-mode .secondary-node,
[data-theme='dark'] .secondary-node {
  background: linear-gradient(135deg, var(--success-color-dark), #2f855a);
  border-color: var(--success-color-dark);
}

.node-group {
  display: flex;
  flex-wrap: wrap;
  justify-content: center;
  gap: 1.25rem;
  max-width: 900px;
}

.connector {
  width: 3px;
  height: 40px;
  background: linear-gradient(to bottom, var(--primary-color-light), transparent);
  margin: 10px 0;
  position: relative;
}

html[data-theme='dark'] .connector,
.dark-mode .connector,
[data-theme='dark'] .connector {
  background: linear-gradient(to bottom, var(--primary-color-dark), transparent);
}

.connector::after {
  content: '';
  position: absolute;
  bottom: -8px;
  left: 50%;
  transform: translateX(-50%);
  width: 0;
  height: 0;
  border-left: 6px solid transparent;
  border-right: 6px solid transparent;
  border-top: 8px solid var(--primary-color-light);
}

html[data-theme='dark'] .connector::after,
.dark-mode .connector::after,
[data-theme='dark'] .connector::after {
  border-top-color: var(--primary-color-dark);
}

/* ============================================
   MULTIMODAL FLOW STYLES
   ============================================ */

.multimodal-flow {
  display: flex;
  flex-direction: column;
  align-items: center;
  gap: 2rem;
}

.flow-row {
  display: flex;
  justify-content: center;
  gap: 2.5rem;
  flex-wrap: wrap;
}

.modality-node {
  display: flex;
  flex-direction: column;
  align-items: center;
  padding: 1.5rem;
  background: var(--node-bg-light);
  border-radius: 16px;
  box-shadow: 0 4px 12px var(--shadow-light);
  min-width: 140px;
  transition: all 0.3s ease;
  border: 2px solid transparent;
}

html[data-theme='dark'] .modality-node,
.dark-mode .modality-node,
[data-theme='dark'] .modality-node {
  background: var(--node-bg-dark);
  box-shadow: 0 4px 16px var(--shadow-dark);
}

.modality-node:hover {
  transform: translateY(-4px) scale(1.05);
  border-color: var(--primary-color-light);
  box-shadow: 0 8px 20px var(--shadow-light);
}

html[data-theme='dark'] .modality-node:hover,
.dark-mode .modality-node:hover,
[data-theme='dark'] .modality-node:hover {
  border-color: var(--primary-color-dark);
  box-shadow: 0 8px 24px var(--shadow-dark);
}

.modality-icon {
  font-size: 2.5rem;
  margin-bottom: 0.75rem;
  filter: grayscale(0.2);
}

.modality-text {
  text-align: center;
  font-weight: 600;
  color: var(--text-primary-light);
  line-height: 1.4;
}

html[data-theme='dark'] .modality-text,
.dark-mode .modality-text,
[data-theme='dark'] .modality-text {
  color: var(--text-primary-dark);
}

.fusion-node {
  background: linear-gradient(135deg, #6f42c1, #553098);
  color: white;
  padding: 1.25rem 3rem;
  border-radius: 30px;
  font-weight: bold;
  font-size: 1.1em;
  box-shadow: 0 4px 12px rgba(111, 66, 193, 0.3);
  transition: all 0.3s ease;
}

html[data-theme='dark'] .fusion-node,
.dark-mode .fusion-node,
[data-theme='dark'] .fusion-node {
  background: linear-gradient(135deg, #805ad5, #6b46c1);
  box-shadow: 0 4px 16px rgba(128, 90, 213, 0.4);
}

.fusion-node:hover {
  transform: scale(1.05);
  box-shadow: 0 6px 20px rgba(111, 66, 193, 0.4);
}

.result-node {
  background: linear-gradient(135deg, var(--success-color-light), #1e7e34);
  color: white;
  padding: 1.25rem 2.5rem;
  border-radius: 12px;
  font-weight: bold;
  font-size: 1.05em;
  box-shadow: 0 4px 12px rgba(40, 167, 69, 0.3);
  transition: all 0.3s ease;
}

html[data-theme='dark'] .result-node,
.dark-mode .result-node,
[data-theme='dark'] .result-node {
  background: linear-gradient(135deg, var(--success-color-dark), #2f855a);
  box-shadow: 0 4px 16px rgba(72, 187, 120, 0.4);
}

.flow-arrow {
  font-size: 2rem;
  color: var(--primary-color-light);
  font-weight: bold;
  text-shadow: 0 2px 4px var(--shadow-light);
}

html[data-theme='dark'] .flow-arrow,
.dark-mode .flow-arrow,
[data-theme='dark'] .flow-arrow {
  color: var(--primary-color-dark);
  text-shadow: 0 2px 4px var(--shadow-dark);
}

/* ============================================
   ARCHITECTURE DIAGRAM STYLES
   ============================================ */

.architecture-diagram {
  display: flex;
  flex-direction: column;
  align-items: center;
  gap: 1.5rem;
  max-width: 800px;
  margin: 0 auto;
}

.arch-node {
  background: var(--node-bg-light);
  border: 3px solid;
  border-radius: 12px;
  padding: 1.5rem 2.5rem;
  text-align: center;
  box-shadow: 0 4px 12px var(--shadow-light);
  width: 100%;
  max-width: 500px;
  transition: all 0.3s ease;
}

html[data-theme='dark'] .arch-node,
.dark-mode .arch-node,
[data-theme='dark'] .arch-node {
  background: var(--node-bg-dark);
  box-shadow: 0 4px 16px var(--shadow-dark);
}

.arch-node:hover {
  transform: translateX(4px);
}

.input-node { 
  border-color: #007acc; 
  background: linear-gradient(135deg, #e3f2fd, #bbdefb);
}
html[data-theme='dark'] .input-node,
.dark-mode .input-node,
[data-theme='dark'] .input-node {
  background: linear-gradient(135deg, #1e3a5f, #2c5282);
}

.process-node { 
  border-color: #ff6b35; 
  background: linear-gradient(135deg, #fff3e0, #ffe0b2);
}
html[data-theme='dark'] .process-node,
.dark-mode .process-node,
[data-theme='dark'] .process-node {
  background: linear-gradient(135deg, #744210, #975a16);
}

.fusion-node.arch-node { 
  border-color: #6f42c1; 
  background: linear-gradient(135deg, #f3e8ff, #e9d5ff);
}
html[data-theme='dark'] .fusion-node.arch-node,
.dark-mode .fusion-node.arch-node,
[data-theme='dark'] .fusion-node.arch-node {
  background: linear-gradient(135deg, #44337a, #553098);
}

.classifier-node { 
  border-color: #28a745; 
  background: linear-gradient(135deg, #e8f5e8, #c8e6c9);
}
html[data-theme='dark'] .classifier-node,
.dark-mode .classifier-node,
[data-theme='dark'] .classifier-node {
  background: linear-gradient(135deg, #1c4532, #276749);
}

.output-node { 
  border-color: #17a2b8; 
  background: linear-gradient(135deg, #e3f2f8, #b3e5fc);
}
html[data-theme='dark'] .output-node,
.dark-mode .output-node,
[data-theme='dark'] .output-node {
  background: linear-gradient(135deg, #1a4d5c, #2c5f75);
}

.arch-title {
  font-weight: bold;
  font-size: 1.15em;
  color: var(--text-primary-light);
  margin-bottom: 0.5rem;
}

html[data-theme='dark'] .arch-title,
.dark-mode .arch-title,
[data-theme='dark'] .arch-title {
  color: var(--text-primary-dark);
}

.arch-subtitle {
  font-size: 0.95em;
  color: var(--text-secondary-light);
  margin-top: 0.5rem;
}

html[data-theme='dark'] .arch-subtitle,
.dark-mode .arch-subtitle,
[data-theme='dark'] .arch-subtitle {
  color: var(--text-secondary-dark);
}

.arch-row {
  display: flex;
  justify-content: center;
  gap: 1.5rem;
  flex-wrap: wrap;
  width: 100%;
  max-width: 700px;
}

.arch-module {
  background: var(--node-bg-light);
  border: 2px solid var(--diagram-border-light);
  border-radius: 10px;
  padding: 1.25rem;
  text-align: center;
  flex: 1;
  min-width: 160px;
  box-shadow: 0 2px 8px var(--shadow-light);
  transition: all 0.3s ease;
}

html[data-theme='dark'] .arch-module,
.dark-mode .arch-module,
[data-theme='dark'] .arch-module {
  background: var(--node-bg-dark);
  border-color: var(--diagram-border-dark);
  box-shadow: 0 2px 12px var(--shadow-dark);
}

.arch-module:hover {
  transform: translateY(-2px);
  border-color: var(--primary-color-light);
  box-shadow: 0 4px 12px var(--shadow-light);
}

html[data-theme='dark'] .arch-module:hover,
.dark-mode .arch-module:hover,
[data-theme='dark'] .arch-module:hover {
  border-color: var(--primary-color-dark);
  box-shadow: 0 4px 16px var(--shadow-dark);
}

.module-title {
  font-weight: bold;
  color: var(--text-primary-light);
  margin-bottom: 0.5rem;
}

html[data-theme='dark'] .module-title,
.dark-mode .module-title,
[data-theme='dark'] .module-title {
  color: var(--text-primary-dark);
}

.module-detail {
  font-size: 0.9em;
  color: var(--text-secondary-light);
  margin-top: 0.5rem;
}

html[data-theme='dark'] .module-detail,
.dark-mode .module-detail,
[data-theme='dark'] .module-detail {
  color: var(--text-secondary-dark);
}

.arch-arrow {
  font-size: 2rem;
  color: var(--text-secondary-light);
  font-weight: bold;
}

html[data-theme='dark'] .arch-arrow,
.dark-mode .arch-arrow,
[data-theme='dark'] .arch-arrow {
  color: var(--text-secondary-dark);
}

/* ============================================
   METHODOLOGY DIAGRAM STYLES
   ============================================ */

.methodology-diagram {
  display: flex;
  flex-direction: column;
  align-items: center;
  gap: 1.5rem;
  max-width: 700px;
  margin: 0 auto;
}

.phase {
  display: flex;
  align-items: center;
  gap: 1.5rem;
  width: 100%;
}

.phase-number {
  background: linear-gradient(135deg, var(--primary-color-light), #0056b3);
  color: white;
  width: 50px;
  height: 50px;
  border-radius: 50%;
  display: flex;
  align-items: center;
  justify-content: center;
  font-weight: bold;
  font-size: 1.2em;
  flex-shrink: 0;
  box-shadow: 0 4px 12px rgba(0, 122, 204, 0.3);
  transition: all 0.3s ease;
}

html[data-theme='dark'] .phase-number,
.dark-mode .phase-number,
[data-theme='dark'] .phase-number {
  background: linear-gradient(135deg, var(--primary-color-dark), #2c5282);
  box-shadow: 0 4px 12px rgba(66, 153, 225, 0.4);
}

.phase:hover .phase-number {
  transform: scale(1.1) rotate(360deg);
}

.phase-content {
  background: var(--node-bg-light);
  border: 2px solid var(--primary-color-light);
  border-radius: 12px;
  padding: 1.25rem;
  flex-grow: 1;
  box-shadow: 0 4px 12px var(--shadow-light);
  transition: all 0.3s ease;
}

html[data-theme='dark'] .phase-content,
.dark-mode .phase-content,
[data-theme='dark'] .phase-content {
  background: var(--node-bg-dark);
  border-color: var(--primary-color-dark);
  box-shadow: 0 4px 16px var(--shadow-dark);
}

.phase:hover .phase-content {
  transform: translateX(4px);
  border-color: var(--success-color-light);
}

html[data-theme='dark'] .phase:hover .phase-content,
.dark-mode .phase:hover .phase-content,
[data-theme='dark'] .phase:hover .phase-content {
  border-color: var(--success-color-dark);
}

.phase-title {
  font-weight: bold;
  text-align: center;
  color: var(--text-primary-light);
}

html[data-theme='dark'] .phase-title,
.dark-mode .phase-title,
[data-theme='dark'] .phase-title {
  color: var(--text-primary-dark);
}

.phase-group {
  display: flex;
  justify-content: center;
  gap: 1.25rem;
  flex-wrap: wrap;
  width: 100%;
}

.phase-sub {
  background: var(--node-bg-light);
  border: 2px solid var(--success-color-light);
  border-radius: 10px;
  padding: 1rem 1.25rem;
  text-align: center;
  flex: 1;
  min-width: 170px;
  box-shadow: 0 2px 8px var(--shadow-light);
  transition: all 0.3s ease;
}

html[data-theme='dark'] .phase-sub,
.dark-mode .phase-sub,
[data-theme='dark'] .phase-sub {
  background: var(--node-bg-dark);
  border-color: var(--success-color-dark);
  box-shadow: 0 2px 12px var(--shadow-dark);
}

.phase-sub:hover {
  transform: translateY(-2px);
  box-shadow: 0 4px 12px var(--shadow-light);
}

html[data-theme='dark'] .phase-sub:hover,
.dark-mode .phase-sub:hover,
[data-theme='dark'] .phase-sub:hover {
  box-shadow: 0 4px 16px var(--shadow-dark);
}

.phase-sub-title {
  font-size: 0.95em;
  font-weight: 600;
  color: var(--text-primary-light);
}

html[data-theme='dark'] .phase-sub-title,
.dark-mode .phase-sub-title,
[data-theme='dark'] .phase-sub-title {
  color: var(--text-primary-dark);
}

.phase-arrow {
  font-size: 2rem;
  color: var(--primary-color-light);
  font-weight: bold;
}

html[data-theme='dark'] .phase-arrow,
.dark-mode .phase-arrow,
[data-theme='dark'] .phase-arrow {
  color: var(--primary-color-dark);
}

/* ============================================
   INTERVENTION FLOW STYLES
   ============================================ */

.intervention-flow {
  display: flex;
  flex-direction: column;
  align-items: center;
  gap: 2rem;
}

.intervention-step {
  display: flex;
  flex-direction: column;
  align-items: center;
  background: var(--node-bg-light);
  border: 3px solid var(--primary-color-light);
  border-radius: 16px;
  padding: 1.5rem 2.5rem;
  box-shadow: 0 4px 12px var(--shadow-light);
  min-width: 180px;
  transition: all 0.3s ease;
}

html[data-theme='dark'] .intervention-step,
.dark-mode .intervention-step,
[data-theme='dark'] .intervention-step {
  background: var(--node-bg-dark);
  border-color: var(--primary-color-dark);
  box-shadow: 0 4px 16px var(--shadow-dark);
}

.intervention-step:hover {
  transform: scale(1.05);
  box-shadow: 0 6px 20px var(--shadow-light);
}

html[data-theme='dark'] .intervention-step:hover,
.dark-mode .intervention-step:hover,
[data-theme='dark'] .intervention-step:hover {
  box-shadow: 0 6px 24px var(--shadow-dark);
}

.step-icon {
  font-size: 2.5rem;
  margin-bottom: 0.75rem;
}

.step-text {
  font-weight: bold;
  text-align: center;
  color: var(--text-primary-light);
}

html[data-theme='dark'] .step-text,
.dark-mode .step-text,
[data-theme='dark'] .step-text {
  color: var(--text-primary-dark);
}

.intervention-step.final {
  background: linear-gradient(135deg, var(--success-color-light), #1e7e34);
  color: white;
  border-color: var(--success-color-light);
}

html[data-theme='dark'] .intervention-step.final,
.dark-mode .intervention-step.final,
[data-theme='dark'] .intervention-step.final {
  background: linear-gradient(135deg, var(--success-color-dark), #2f855a);
  border-color: var(--success-color-dark);
}

.intervention-step.final .step-text {
  color: white;
}

.priority-group {
  display: flex;
  justify-content: center;
  gap: 1.5rem;
  flex-wrap: wrap;
  width: 100%;
  max-width: 900px;
}

.priority-item {
  background: var(--node-bg-light);
  border: 3px solid;
  border-radius: 12px;
  padding: 1.25rem;
  text-align: center;
  flex: 1;
  min-width: 140px;
  box-shadow: 0 4px 12px var(--shadow-light);
  transition: all 0.3s ease;
}

html[data-theme='dark'] .priority-item,
.dark-mode .priority-item,
[data-theme='dark'] .priority-item {
  box-shadow: 0 4px 16px var(--shadow-dark);
}

.priority-item:hover {
  transform: translateY(-4px);
  box-shadow: 0 6px 16px var(--shadow-light);
}

html[data-theme='dark'] .priority-item:hover,
.dark-mode .priority-item:hover,
[data-theme='dark'] .priority-item:hover {
  box-shadow: 0 6px 20px var(--shadow-dark);
}

.priority-item.mild { 
  border-color: var(--warning-color-light); 
  background: linear-gradient(135deg, #fffbf0, #fff9e6);
}
html[data-theme='dark'] .priority-item.mild,
.dark-mode .priority-item.mild,
[data-theme='dark'] .priority-item.mild {
  background: linear-gradient(135deg, #744d00, #975f00);
}

.priority-item.moderate { 
  border-color: #fd7e14; 
  background: linear-gradient(135deg, #fff4e6, #ffe8cc);
}
html[data-theme='dark'] .priority-item.moderate,
.dark-mode .priority-item.moderate,
[data-theme='dark'] .priority-item.moderate {
  background: linear-gradient(135deg, #7d3f0a, #a14e0b);
}

.priority-item.severe { 
  border-color: var(--danger-color-light); 
  background: linear-gradient(135deg, #ffe6e6, #ffcccc);
}
html[data-theme='dark'] .priority-item.severe,
.dark-mode .priority-item.severe,
[data-theme='dark'] .priority-item.severe {
  background: linear-gradient(135deg, #742b2b, #9b3636);
}

.priority-title {
  font-weight: bold;
  margin-bottom: 0.5rem;
  color: var(--text-primary-light);
}

html[data-theme='dark'] .priority-title,
.dark-mode .priority-title,
[data-theme='dark'] .priority-title {
  color: var(--text-primary-dark);
}

.priority-desc {
  font-size: 0.9em;
  color: var(--text-secondary-light);
}

html[data-theme='dark'] .priority-desc,
.dark-mode .priority-desc,
[data-theme='dark'] .priority-desc {
  color: var(--text-secondary-dark);
}

.step-arrow {
  font-size: 2rem;
  color: var(--primary-color-light);
  font-weight: bold;
}

html[data-theme='dark'] .step-arrow,
.dark-mode .step-arrow,
[data-theme='dark'] .step-arrow {
  color: var(--primary-color-dark);
}

/* ============================================
   CHART STYLES
   ============================================ */

.chart-container {
  margin: 3rem 0;
}

.accuracy-chart {
  background: var(--node-bg-light);
  border-radius: 16px;
  padding: 2.5rem;
  box-shadow: 0 4px 16px var(--shadow-light);
  transition: all 0.3s ease;
}

html[data-theme='dark'] .accuracy-chart,
.dark-mode .accuracy-chart,
[data-theme='dark'] .accuracy-chart {
  background: var(--node-bg-dark);
  box-shadow: 0 4px 20px var(--shadow-dark);
}

.chart-title {
  font-weight: bold;
  text-align: center;
  margin-bottom: 2.5rem;
  font-size: 1.2em;
  color: var(--text-primary-light);
}

html[data-theme='dark'] .chart-title,
.dark-mode .chart-title,
[data-theme='dark'] .chart-title {
  color: var(--text-primary-dark);
}

.chart-bars {
  display: flex;
  flex-direction: column;
  gap: 2rem;
}

.bar-container {
  display: flex;
  align-items: center;
  gap: 1.5rem;
}

.bar-label {
  min-width: 120px;
  font-weight: 600;
  text-align: right;
  color: var(--text-primary-light);
}

html[data-theme='dark'] .bar-label,
.dark-mode .bar-label,
[data-theme='dark'] .bar-label {
  color: var(--text-primary-dark);
}

.bar-wrapper {
  flex-grow: 1;
  background: var(--diagram-border-light);
  border-radius: 25px;
  height: 35px;
  position: relative;
  overflow: hidden;
}

html[data-theme='dark'] .bar-wrapper,
.dark-mode .bar-wrapper,
[data-theme='dark'] .bar-wrapper {
  background: var(--diagram-border-dark);
}

.bar {
  height: 100%;
  border-radius: 25px;
  display: flex;
  align-items: center;
  justify-content: flex-end;
  padding: 0 1.25rem;
  transition: width 1s cubic-bezier(0.4, 0, 0.2, 1);
  position: relative;
  overflow: hidden;
}

.bar::before {
  content: '';
  position: absolute;
  top: 0;
  left: -100%;
  width: 100%;
  height: 100%;
  background: linear-gradient(90deg, transparent, rgba(255,255,255,0.3), transparent);
  animation: shimmer 2s infinite;
}

@keyframes shimmer {
  100% { left: 100%; }
}

.bar-1 { background: linear-gradient(90deg, #4facfe 0%, #00f2fe 100%); }
.bar-2 { background: linear-gradient(90deg, #43e97b 0%, #38f9d7 100%); }
.bar-3 { background: linear-gradient(90deg, #fa709a 0%, #fee140 100%); }
.bar-4 { background: linear-gradient(90deg, #667eea 0%, #764ba2 100%); }

html[data-theme='dark'] .bar-1,
.dark-mode .bar-1,
[data-theme='dark'] .bar-1 { 
  background: linear-gradient(90deg, #2d7ab8 0%, #0099cc 100%); 
}

html[data-theme='dark'] .bar-2,
.dark-mode .bar-2,
[data-theme='dark'] .bar-2 { 
  background: linear-gradient(90deg, #2a9858 0%, #25b48a 100%); 
}

html[data-theme='dark'] .bar-3,
.dark-mode .bar-3,
[data-theme='dark'] .bar-3 { 
  background: linear-gradient(90deg, #c84a6f 0%, #d4a933 100%); 
}

html[data-theme='dark'] .bar-4,
.dark-mode .bar-4,
[data-theme='dark'] .bar-4 { 
  background: linear-gradient(90deg, #4d5fb8 0%, #5a3a7e 100%); 
}

.bar-value {
  color: white;
  font-weight: bold;
  font-size: 1em;
  text-shadow: 1px 1px 3px rgba(0,0,0,0.4);
  position: relative;
  z-index: 1;
}

/* ============================================
   ETHICS DIAGRAM STYLES
   ============================================ */

.ethics-diagram {
  display: flex;
  flex-direction: column;
  align-items: center;
  gap: 3rem;
}

.ethics-center {
  background: linear-gradient(135deg, var(--primary-color-light), #0056b3);
  color: white;
  padding: 2rem 3rem;
  border-radius: 50%;
  font-weight: bold;
  font-size: 1.15em;
  text-align: center;
  box-shadow: 0 6px 20px rgba(0, 122, 204, 0.4);
  transition: all 0.3s ease;
  max-width: 250px;
}

html[data-theme='dark'] .ethics-center,
.dark-mode .ethics-center,
[data-theme='dark'] .ethics-center {
  background: linear-gradient(135deg, var(--primary-color-dark), #2c5282);
  box-shadow: 0 6px 24px rgba(66, 153, 225, 0.5);
}

.ethics-center:hover {
  transform: scale(1.05) rotate(5deg);
}

.ethics-branches {
  display: flex;
  justify-content: center;
  gap: 2.5rem;
  flex-wrap: wrap;
  max-width: 1000px;
}

.ethics-branch {
  display: flex;
  flex-direction: column;
  align-items: center;
  gap: 1.25rem;
  flex: 1;
  min-width: 220px;
}

.ethics-node {
  background: var(--node-bg-light);
  border: 3px solid var(--success-color-light);
  border-radius: 12px;
  padding: 1.25rem;
  text-align: center;
  box-shadow: 0 4px 12px var(--shadow-light);
  width: 100%;
  transition: all 0.3s ease;
}

html[data-theme='dark'] .ethics-node,
.dark-mode .ethics-node,
[data-theme='dark'] .ethics-node {
  background: var(--node-bg-dark);
  border-color: var(--success-color-dark);
  box-shadow: 0 4px 16px var(--shadow-dark);
}

.ethics-node:hover {
  transform: translateY(-4px);
  box-shadow: 0 6px 16px var(--shadow-light);
}

html[data-theme='dark'] .ethics-node:hover,
.dark-mode .ethics-node:hover,
[data-theme='dark'] .ethics-node:hover {
  box-shadow: 0 6px 20px var(--shadow-dark);
}

.ethics-title {
  font-weight: bold;
  color: var(--text-primary-light);
}

html[data-theme='dark'] .ethics-title,
.dark-mode .ethics-title,
[data-theme='dark'] .ethics-title {
  color: var(--text-primary-dark);
}

.ethics-leaf {
  background: var(--diagram-bg-light);
  border: 2px solid var(--diagram-border-light);
  border-radius: 10px;
  padding: 1rem;
  text-align: center;
  width: 100%;
  transition: all 0.3s ease;
}

html[data-theme='dark'] .ethics-leaf,
.dark-mode .ethics-leaf,
[data-theme='dark'] .ethics-leaf {
  background: var(--diagram-bg-dark);
  border-color: var(--diagram-border-dark);
}

.leaf-text {
  font-size: 0.95em;
  color: var(--text-secondary-light);
}

html[data-theme='dark'] .leaf-text,
.dark-mode .leaf-text,
[data-theme='dark'] .leaf-text {
  color: var(--text-secondary-dark);
}

.branch-line {
  width: 3px;
  height: 40px;
  background: linear-gradient(to bottom, var(--success-color-light), transparent);
  position: relative;
}

html[data-theme='dark'] .branch-line,
.dark-mode .branch-line,
[data-theme='dark'] .branch-line {
  background: linear-gradient(to bottom, var(--success-color-dark), transparent);
}

.branch-line::after {
  content: '';
  position: absolute;
  bottom: -8px;
  left: 50%;
  transform: translateX(-50%);
  width: 0;
  height: 0;
  border-left: 6px solid transparent;
  border-right: 6px solid transparent;
  border-top: 8px solid var(--success-color-light);
}

html[data-theme='dark'] .branch-line::after,
.dark-mode .branch-line::after,
[data-theme='dark'] .branch-line::after {
  border-top-color: var(--success-color-dark);
}

/* ============================================
   TABLE STYLES
   ============================================ */

.table-container {
  margin: 3rem 0;
  overflow-x: auto;
  border-radius: 12px;
  box-shadow: 0 4px 16px var(--shadow-light);
}

html[data-theme='dark'] .table-container,
.dark-mode .table-container,
[data-theme='dark'] .table-container {
  box-shadow: 0 4px 20px var(--shadow-dark);
}

.products-table {
  width: 100%;
  border-collapse: collapse;
  background: var(--node-bg-light);
  border-radius: 12px;
  overflow: hidden;
}

html[data-theme='dark'] .products-table,
.dark-mode .products-table,
[data-theme='dark'] .products-table {
  background: var(--node-bg-dark);
}

.products-table th {
  background: linear-gradient(135deg, var(--primary-color-light), #0056b3);
  color: white;
  padding: 1.25rem;
  text-align: left;
  font-weight: bold;
  font-size: 1.05em;
}

html[data-theme='dark'] .products-table th,
.dark-mode .products-table th,
[data-theme='dark'] .products-table th {
  background: linear-gradient(135deg, var(--primary-color-dark), #2c5282);
}

.products-table td {
  padding: 1.25rem;
  border-bottom: 1px solid var(--diagram-border-light);
  vertical-align: top;
  color: var(--text-primary-light);
  line-height: 1.6;
}

html[data-theme='dark'] .products-table td,
.dark-mode .products-table td,
[data-theme='dark'] .products-table td {
  border-bottom-color: var(--diagram-border-dark);
  color: var(--text-primary-dark);
}

.products-table tr {
  transition: background-color 0.2s ease;
}

.products-table tr:hover {
  background: var(--diagram-bg-light);
}

html[data-theme='dark'] .products-table tr:hover,
.dark-mode .products-table tr:hover,
[data-theme='dark'] .products-table tr:hover {
  background: var(--diagram-bg-dark);
}

.products-table tr:last-child td {
  border-bottom: none;
}

.products-table strong {
  color: var(--primary-color-light);
  font-weight: 600;
}

html[data-theme='dark'] .products-table strong,
.dark-mode .products-table strong,
[data-theme='dark'] .products-table strong {
  color: var(--primary-color-dark);
}

/* ============================================
   RESPONSIVE DESIGN
   ============================================ */

@media (max-width: 1024px) {
  .diagram-container {
    padding: 1.5rem;
    margin: 2rem 0;
  }
  
  .node-group, .flow-row, .arch-row, .phase-group, 
  .priority-group, .ethics-branches {
    gap: 1rem;
  }
}

@media (max-width: 768px) {
  .diagram-container {
    padding: 1.25rem;
    margin: 1.5rem 0;
    border-radius: 12px;
  }
  
  .node-group, .flow-row, .arch-row, .phase-group, 
  .priority-group, .ethics-branches {
    flex-direction: column;
    align-items: center;
  }
  
  .node, .arch-module, .phase-sub, .priority-item {
    min-width: 240px;
    max-width: 100%;
  }
  
  .bar-container {
    flex-direction: column;
    align-items: flex-start;
    gap: 0.75rem;
  }
  
  .bar-label {
    min-width: auto;
    text-align: left;
  }
  
  .phase {
    flex-direction: column;
    align-items: center;
    text-align: center;
  }
  
  .phase-number {
    width: 45px;
    height: 45px;
    font-size: 1.1em;
  }
  
  .modality-icon {
    font-size: 2rem;
  }
  
  .step-icon {
    font-size: 2rem;
  }
  
  .accuracy-chart {
    padding: 1.5rem;
  }
  
  .chart-title {
    font-size: 1.05em;
    margin-bottom: 1.5rem;
  }
  
  .products-table {
    font-size: 0.9em;
  }
  
  .products-table th,
  .products-table td {
    padding: 1rem;
  }
}

@media (max-width: 480px) {
  .diagram-container {
    padding: 1rem;
    margin: 1rem 0;
  }
  
  .node, .arch-module, .phase-sub, .priority-item,
  .intervention-step {
    min-width: 200px;
    padding: 1rem;
  }
  
  .main-node, .fusion-node, .result-node {
    font-size: 1em;
    padding: 1rem 1.5rem;
  }
  
  .arch-title {
    font-size: 1em;
  }
  
  .flow-arrow, .arch-arrow, .phase-arrow, .step-arrow {
    font-size: 1.5rem;
  }
  
  .chart-bars {
    gap: 1.5rem;
  }
  
  .bar-wrapper {
    height: 30px;
  }
  
  .bar-value {
    font-size: 0.9em;
  }
  
  .ethics-center {
    padding: 1.5rem 2rem;
    font-size: 1em;
    max-width: 200px;
  }
}

/* ============================================
   ACCESSIBILITY
   ============================================ */

@media (prefers-reduced-motion: reduce) {
  * {
    animation-duration: 0.01ms !important;
    animation-iteration-count: 1 !important;
    transition-duration: 0.01ms !important;
  }
  
  .bar::before {
    animation: none;
  }
}

/* Focus styles for accessibility */
.node:focus,
.arch-node:focus,
.phase-content:focus,
.priority-item:focus,
.ethics-node:focus {
  outline: 3px solid var(--primary-color-light);
  outline-offset: 2px;
}

html[data-theme='dark'] .node:focus,
html[data-theme='dark'] .arch-node:focus,
html[data-theme='dark'] .phase-content:focus,
html[data-theme='dark'] .priority-item:focus,
html[data-theme='dark'] .ethics-node:focus,
.dark-mode .node:focus,
.dark-mode .arch-node:focus,
.dark-mode .phase-content:focus,
.dark-mode .priority-item:focus,
.dark-mode .ethics-node:focus,
[data-theme='dark'] .node:focus,
[data-theme='dark'] .arch-node:focus,
[data-theme='dark'] .phase-content:focus,
[data-theme='dark'] .priority-item:focus,
[data-theme='dark'] .ethics-node:focus {
  outline-color: var(--primary-color-dark);
}

/* Print styles */
@media print {
  .diagram-container {
    break-inside: avoid;
    box-shadow: none;
    border: 1px solid #000;
  }
  
  .node, .arch-node, .phase-content, .priority-item {
    box-shadow: none;
  }
}
</style>
