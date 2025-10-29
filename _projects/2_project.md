---
layout: page
title: Early Detection of Depression and Anxiety
description: Multimodal System for Early Detection of Depression and Anxiety in University Population
img: assets/img/banner-thesis-jeison.jpg
importance: 2
category: work
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
      <div class="step-text">Resource Optimization University Welfare</div>
    </div>
  </div>
</div>

**Initial target population:** Systems Engineering and Psychology students from Universidad Tecnológica de Bolívar, with potential for expansion to other faculties and institutions.

## Scientific and Technical Contribution

This project represents several significant contributions to the field of automated mental health problem detection:

**Technical innovation:** Development of adaptive multimodal fusion strategies that dynamically adjust the weights of each modality according to individual patterns, overcoming the limitations of fixed fusion approaches.

**Data contribution:** Creation of the first multimodal corpus in Spanish specifically for Colombian university context, labeled with validated scales (PHQ-9 and GAD-7) and available to the scientific community.

**Methodological advancement:** Establishment of specialized ethical protocols for collection and processing of sensitive multimodal data in educational environments.

<div class="chart-container">
  <div class="accuracy-chart">
    <div class="chart-title">Accuracy Comparison Between Unimodal and Multimodal Approaches</div>
    <div class="chart-bars">
      <div class="bar-container">
        <div class="bar-label">Text Only</div>
        <div class="bar-wrapper">
          <div class="bar bar-1" style="width: 65%">
            <span class="bar-value">65%</span>
          </div>
        </div>
      </div>
      <div class="bar-container">
        <div class="bar-label">Audio Only</div>
        <div class="bar-wrapper">
          <div class="bar bar-2" style="width: 58%">
            <span class="bar-value">58%</span>
          </div>
        </div>
      </div>
      <div class="bar-container">
        <div class="bar-label">Video Only</div>
        <div class="bar-wrapper">
          <div class="bar bar-3" style="width: 62%">
            <span class="bar-value">62%</span>
          </div>
        </div>
      </div>
      <div class="bar-container">
        <div class="bar-label">Multimodal</div>
        <div class="bar-wrapper">
          <div class="bar bar-4" style="width: 82%">
            <span class="bar-value">82%</span>
          </div>
        </div>
      </div>
    </div>
  </div>
</div>

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
          <div class="ethics-title">Informed Consent by Modality</div>
        </div>
        <div class="branch-line"></div>
        <div class="ethics-leaf">
          <div class="leaf-text">Equity in Detection Without Demographic Biases</div>
        </div>
      </div>
      <div class="ethics-branch">
        <div class="branch-line"></div>
        <div class="ethics-node">
          <div class="ethics-title">Anonymization of Sensitive Data</div>
        </div>
        <div class="branch-line"></div>
        <div class="ethics-leaf">
          <div class="leaf-text">Privacy Preserved Identity Protected</div>
        </div>
      </div>
      <div class="ethics-branch">
        <div class="branch-line"></div>
        <div class="ethics-node">
          <div class="ethics-title">Transparency in Data Use</div>
        </div>
        <div class="branch-line"></div>
        <div class="ethics-leaf">
          <div class="leaf-text">Institutional and Student Trust</div>
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

<style>
.diagram-container {
  margin: 2rem 0;
  padding: 1.5rem;
  background: #f8f9fa;
  border-radius: 12px;
  border: 1px solid #e9ecef;
}

/* Crisis Diagram Styles */
.crisis-diagram {
  display: flex;
  flex-direction: column;
  align-items: center;
  gap: 1rem;
}

.node {
  background: white;
  border: 2px solid #007acc;
  border-radius: 8px;
  padding: 1rem;
  margin: 0.5rem;
  text-align: center;
  box-shadow: 0 2px 8px rgba(0,0,0,0.1);
  min-width: 180px;
  font-weight: 500;
}

.main-node {
  background: #007acc;
  color: white;
  font-weight: bold;
  font-size: 1.1em;
}

.secondary-node {
  background: #28a745;
  color: white;
  border-color: #28a745;
}

.node-group {
  display: flex;
  flex-wrap: wrap;
  justify-content: center;
  gap: 1rem;
}

.connector {
  width: 3px;
  height: 30px;
  background: #007acc;
  margin: 10px 0;
}

/* Multimodal Flow Styles */
.multimodal-flow {
  display: flex;
  flex-direction: column;
  align-items: center;
  gap: 1rem;
}

.flow-row {
  display: flex;
  justify-content: center;
  gap: 2rem;
  flex-wrap: wrap;
}

.modality-node {
  display: flex;
  flex-direction: column;
  align-items: center;
  padding: 1rem;
  background: white;
  border-radius: 10px;
  box-shadow: 0 2px 8px rgba(0,0,0,0.1);
  min-width: 120px;
}

.modality-icon {
  font-size: 2rem;
  margin-bottom: 0.5rem;
}

.modality-text {
  text-align: center;
  font-weight: 500;
}

.fusion-node {
  background: #6f42c1;
  color: white;
  padding: 1rem 2rem;
  border-radius: 25px;
  font-weight: bold;
}

.result-node {
  background: #28a745;
  color: white;
  padding: 1rem 2rem;
  border-radius: 10px;
  font-weight: bold;
}

.flow-arrow {
  font-size: 1.5rem;
  color: #007acc;
  font-weight: bold;
}

/* Architecture Diagram Styles */
.architecture-diagram {
  display: flex;
  flex-direction: column;
  align-items: center;
  gap: 1rem;
}

.arch-node {
  background: white;
  border: 2px solid;
  border-radius: 8px;
  padding: 1rem 2rem;
  text-align: center;
  box-shadow: 0 2px 8px rgba(0,0,0,0.1);
  width: 100%;
  max-width: 400px;
}

.input-node { border-color: #007acc; background: #e3f2fd; }
.process-node { border-color: #ff6b35; background: #fff3e0; }
.fusion-node { border-color: #6f42c1; background: #f3e8ff; }
.classifier-node { border-color: #28a745; background: #e8f5e8; }
.output-node { border-color: #17a2b8; background: #e3f2f8; }

.arch-title {
  font-weight: bold;
  font-size: 1.1em;
}

.arch-subtitle {
  font-size: 0.9em;
  opacity: 0.8;
  margin-top: 0.5rem;
}

.arch-row {
  display: flex;
  justify-content: center;
  gap: 1rem;
  flex-wrap: wrap;
  width: 100%;
}

.arch-module {
  background: white;
  border: 1px solid #dee2e6;
  border-radius: 6px;
  padding: 1rem;
  text-align: center;
  flex: 1;
  min-width: 150px;
  box-shadow: 0 1px 4px rgba(0,0,0,0.1);
}

.module-title {
  font-weight: bold;
  color: #495057;
}

.module-detail {
  font-size: 0.85em;
  color: #6c757d;
  margin-top: 0.5rem;
}

.arch-arrow {
  font-size: 1.5rem;
  color: #6c757d;
  font-weight: bold;
}

/* Methodology Diagram Styles */
.methodology-diagram {
  display: flex;
  flex-direction: column;
  align-items: center;
  gap: 1rem;
}

.phase {
  display: flex;
  align-items: center;
  gap: 1rem;
  width: 100%;
  max-width: 500px;
}

.phase-number {
  background: #007acc;
  color: white;
  width: 40px;
  height: 40px;
  border-radius: 50%;
  display: flex;
  align-items: center;
  justify-content: center;
  font-weight: bold;
  flex-shrink: 0;
}

.phase-content {
  background: white;
  border: 2px solid #007acc;
  border-radius: 8px;
  padding: 1rem;
  flex-grow: 1;
  box-shadow: 0 2px 8px rgba(0,0,0,0.1);
}

.phase-title {
  font-weight: bold;
  text-align: center;
}

.phase-group {
  display: flex;
  justify-content: center;
  gap: 1rem;
  flex-wrap: wrap;
  width: 100%;
}

.phase-sub {
  background: white;
  border: 1px solid #28a745;
  border-radius: 6px;
  padding: 0.75rem 1rem;
  text-align: center;
  flex: 1;
  min-width: 150px;
  box-shadow: 0 1px 4px rgba(0,0,0,0.1);
}

.phase-sub-title {
  font-size: 0.9em;
  font-weight: 500;
}

.phase-arrow {
  font-size: 1.5rem;
  color: #007acc;
  font-weight: bold;
}

/* Intervention Flow Styles */
.intervention-flow {
  display: flex;
  flex-direction: column;
  align-items: center;
  gap: 1.5rem;
}

.intervention-step {
  display: flex;
  flex-direction: column;
  align-items: center;
  background: white;
  border: 2px solid #007acc;
  border-radius: 10px;
  padding: 1rem 2rem;
  box-shadow: 0 2px 8px rgba(0,0,0,0.1);
  min-width: 150px;
}

.step-icon {
  font-size: 2rem;
  margin-bottom: 0.5rem;
}

.step-text {
  font-weight: bold;
  text-align: center;
}

.intervention-step.final {
  background: #28a745;
  color: white;
  border-color: #28a745;
}

.priority-group {
  display: flex;
  justify-content: center;
  gap: 1rem;
  flex-wrap: wrap;
  width: 100%;
}

.priority-item {
  background: white;
  border: 2px solid;
  border-radius: 8px;
  padding: 1rem;
  text-align: center;
  flex: 1;
  min-width: 120px;
  box-shadow: 0 2px 8px rgba(0,0,0,0.1);
}

.priority-item.mild { border-color: #ffc107; background: #fffbf0; }
.priority-item.moderate { border-color: #fd7e14; background: #fff4e6; }
.priority-item.severe { border-color: #dc3545; background: #ffe6e6; }

.priority-title {
  font-weight: bold;
  margin-bottom: 0.5rem;
}

.priority-desc {
  font-size: 0.85em;
  color: #6c757d;
}

.step-arrow {
  font-size: 1.5rem;
  color: #007acc;
  font-weight: bold;
}

/* Chart Styles */
.chart-container {
  margin: 2rem 0;
}

.accuracy-chart {
  background: white;
  border-radius: 12px;
  padding: 2rem;
  box-shadow: 0 4px 12px rgba(0,0,0,0.1);
}

.chart-title {
  font-weight: bold;
  text-align: center;
  margin-bottom: 2rem;
  font-size: 1.1em;
  color: #495057;
}

.chart-bars {
  display: flex;
  flex-direction: column;
  gap: 1.5rem;
}

.bar-container {
  display: flex;
  align-items: center;
  gap: 1rem;
}

.bar-label {
  min-width: 100px;
  font-weight: 500;
  text-align: right;
}

.bar-wrapper {
  flex-grow: 1;
  background: #e9ecef;
  border-radius: 20px;
  height: 30px;
  position: relative;
  overflow: hidden;
}

.bar {
  height: 100%;
  border-radius: 20px;
  display: flex;
  align-items: center;
  justify-content: flex-end;
  padding: 0 1rem;
  transition: width 0.5s ease;
}

.bar-1 { background: linear-gradient(90deg, #4facfe 0%, #00f2fe 100%); }
.bar-2 { background: linear-gradient(90deg, #43e97b 0%, #38f9d7 100%); }
.bar-3 { background: linear-gradient(90deg, #fa709a 0%, #fee140 100%); }
.bar-4 { background: linear-gradient(90deg, #667eea 0%, #764ba2 100%); }

.bar-value {
  color: white;
  font-weight: bold;
  font-size: 0.9em;
  text-shadow: 1px 1px 2px rgba(0,0,0,0.3);
}

/* Ethics Diagram Styles */
.ethics-diagram {
  display: flex;
  flex-direction: column;
  align-items: center;
  gap: 2rem;
}

.ethics-center {
  background: #007acc;
  color: white;
  padding: 1.5rem 2rem;
  border-radius: 50%;
  font-weight: bold;
  text-align: center;
  box-shadow: 0 4px 12px rgba(0,0,0,0.2);
}

.ethics-branches {
  display: flex;
  justify-content: center;
  gap: 2rem;
  flex-wrap: wrap;
}

.ethics-branch {
  display: flex;
  flex-direction: column;
  align-items: center;
  gap: 1rem;
  flex: 1;
  min-width: 200px;
}

.ethics-node {
  background: white;
  border: 2px solid #28a745;
  border-radius: 8px;
  padding: 1rem;
  text-align: center;
  box-shadow: 0 2px 8px rgba(0,0,0,0.1);
  width: 100%;
}

.ethics-title {
  font-weight: bold;
}

.ethics-leaf {
  background: #f8f9fa;
  border: 1px solid #dee2e6;
  border-radius: 6px;
  padding: 0.75rem;
  text-align: center;
  width: 100%;
}

.leaf-text {
  font-size: 0.9em;
  color: #495057;
}

.branch-line {
  width: 2px;
  height: 30px;
  background: #007acc;
}

/* Table Styles */
.table-container {
  margin: 2rem 0;
  overflow-x: auto;
}

.products-table {
  width: 100%;
  border-collapse: collapse;
  background: white;
  border-radius: 8px;
  overflow: hidden;
  box-shadow: 0 4px 12px rgba(0,0,0,0.1);
}

.products-table th {
  background: #007acc;
  color: white;
  padding: 1rem;
  text-align: left;
  font-weight: bold;
}

.products-table td {
  padding: 1rem;
  border-bottom: 1px solid #dee2e6;
  vertical-align: top;
}

.products-table tr:hover {
  background: #f8f9fa;
}

.products-table tr:last-child td {
  border-bottom: none;
}

/* Responsive Design */
@media (max-width: 768px) {
  .diagram-container {
    padding: 1rem;
    margin: 1rem 0;
  }
  
  .node-group, .flow-row, .arch-row, .phase-group, .priority-group, .ethics-branches {
    flex-direction: column;
    align-items: center;
  }
  
  .node, .arch-module, .phase-sub, .priority-item {
    min-width: 200px;
  }
  
  .bar-container {
    flex-direction: column;
    align-items: flex-start;
    gap: 0.5rem;
  }
  
  .bar-label {
    min-width: auto;
    text-align: left;
  }
}
</style>
