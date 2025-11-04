---
layout: page
title: Early Detection of Depression and Anxiety
description: Multimodal System for Early Detection of Depression and Anxiety in University Population
img: assets/img/banner-thesis-jeison.jpg
importance: 3
category: Master's degree
giscus_comments: true
---

# Integrated Methodology for Improving Automatic Translation of Gastronomic Texts through Named Entity Recognition

## General Information

- **Principal Investigator:** Daniel Arturo Peña Gnecco
- **Director:** Juan Carlos Martinez-Santos
- **Co-Director:** Edwin Alexander Puertas del Castillo
- **Program:** Master's in Engineering
- **Research Line:** Natural Language Processing and Applied Artificial Intelligence

## Abstract

In a globalized world, accurate translation of gastronomic texts is essential for promoting cultural exchange and improving the experience of international users. This research develops an integrated methodology that combines Named Entity Recognition (NER) with Neural Machine Translation (NMT) to optimize translation quality between Spanish and English, preserving the cultural and semantic context of gastronomic texts.

## Problem Description

### Context

Gastronomic texts—menus, recipes, culinary reviews, and tourist guides—play a crucial role in intercultural communication. However, current automatic translation systems face significant challenges when processing them, especially when they contain culturally specific named entities.

### Core Problem

Neural Machine Translation (NMT) models tend to generate literal translations that:

- **Omit cultural nuances:** For example, translating "ceviche" as "raw fish" not only ignores the unique preparation of the dish but can also disorient tourists seeking an authentic culinary experience.

- **Lose relevant information:** Elements such as dish names (mole poblano), ingredients (chipotle, dashi), or culinary techniques (sous-vide) are fundamental for conveying the cultural identity and precise meaning of these texts.

- **Generate comprehension errors:** Inaccurate translations in menus or reviews hinder communication in international contexts, affecting the experience of non-native users.

### Technical Challenges

1. **Out-of-vocabulary (OOV) terms:** Exotic ingredients and traditional dish names often generate inaccurate translations due to their low frequency in training data.

2. **Semantic ambiguity:** Cultural context is crucial for adequate translation, but conventional systems prioritize literal translations.

3. **Lack of bilingual resources:** The absence of specialized annotated corpora in the gastronomic domain for the Spanish-English pair limits the training of adapted models.

4. **Separate processes:** Current systems apply NER and MT as independent processes, preventing exploitation of synergies between entity identification and culturally informed translation.

<div style="background: linear-gradient(135deg, #667eea 0%, #764ba2 100%); padding: 25px; border-radius: 10px; margin: 30px 0; color: white;">
  <h4 style="margin-top: 0; text-align: center; color: white;">Comparison: Traditional System vs Proposed System</h4>
  <div style="display: grid; grid-template-columns: 1fr 1fr; gap: 20px; margin-top: 20px;">
    <div style="background: rgba(255,255,255,0.1); padding: 15px; border-radius: 8px; border: 2px solid rgba(255,255,255,0.3);">
      <h5 style="margin-top: 0; color: #ffeb3b;">Traditional System (NMT only)</h5>
      <div style="font-family: monospace; background: rgba(0,0,0,0.3); padding: 10px; border-radius: 5px; margin: 10px 0;">
        "Ceviche de pescado"<br>
        &nbsp;&nbsp;↓ [NMT]<br>
        ✗ "Raw fish ceviche"
      </div>
      <ul style="font-size: 0.9em; line-height: 1.6;">
        <li>Cultural loss</li>
        <li>Literal translation</li>
        <li>Does not identify entities</li>
      </ul>
    </div>
    <div style="background: rgba(255,255,255,0.1); padding: 15px; border-radius: 8px; border: 2px solid #4caf50;">
      <h5 style="margin-top: 0; color: #4caf50;">Proposed System (NER + NMT)</h5>
      <div style="font-family: monospace; background: rgba(0,0,0,0.3); padding: 10px; border-radius: 5px; margin: 10px 0;">
        "Ceviche de pescado"<br>
        &nbsp;&nbsp;↓ [NER] → DISH<br>
        &nbsp;&nbsp;↓ [NMT + Context]<br>
        ✓ "Peruvian ceviche"
      </div>
      <ul style="font-size: 0.9em; line-height: 1.6;">
        <li>Preserves cultural context</li>
        <li>Identifies entities</li>
        <li>Informed translation</li>
      </ul>
    </div>
  </div>
</div>

### Research Question

How can the integration of Named Entity Recognition (NER) in neural machine translation (NMT) systems improve the quality of gastronomic text translations between Spanish and English, ensuring the preservation of cultural and semantic context?

## Objectives

### General Objective

Design and evaluate an integrated methodology that combines Named Entity Recognition (NER) with Neural Machine Translation (NMT) to improve the quality of gastronomic text translations between Spanish and English, preserving cultural and semantic context.

### Specific Objectives

1. Create a bilingual corpus (Spanish-English) of gastronomic texts annotated with named entities (dish names, ingredients, and culinary techniques) and categorize these entities, laying the foundation for developing specialized models.

2. Develop a specialized NER model for the gastronomic domain, trained with the bilingual corpus, capable of recognizing entities with high precision to support contextualized translation.

3. Create a Neural Machine Translation (NMT) model adapted to the gastronomic domain through fine-tuning, integrating the NER model to ensure proper handling of named entities.

4. Evaluate the integrated system using automatic metrics (BLEU and METEOR) and human evaluations, focusing on precision and cultural adequacy.

## Proposed Methodology

The research adopts a quantitative and experimental approach with a comparative design that seeks to evaluate the effectiveness of integrating NER and NMT in gastronomic translation.

### 1. Collection and Annotation of Bilingual Corpus

**Corpus target:** 517,088 balanced sentences between recipes and menus.

**Data sources:**
- Restaurant menus
- Culinary recipes
- Gastronomic reviews
- Gastronomic tourist guides

**Annotation strategy:**

The annotation follows a **sequential two-step process** that balances semantic richness with low cognitive load:

<div style="background: #f5f5f5; border-left: 4px solid #2196F3; padding: 20px; margin: 25px 0; border-radius: 5px;">
  <h4 style="margin-top: 0; color: #2196F3;">Sequential Annotation Process</h4>
  <div style="display: flex; align-items: center; justify-content: space-around; flex-wrap: wrap;">
    <div style="text-align: center; margin: 10px;">
      <div style="background: #e3f2fd; border: 2px solid #2196F3; border-radius: 8px; padding: 15px; min-width: 150px;">
        <div style="font-weight: bold; color: #1976D2; margin-bottom: 10px;">Raw Text</div>
        <div style="font-size: 0.85em; color: #666;">System input</div>
      </div>
    </div>
    <div style="font-size: 24px; color: #2196F3;">→</div>
    <div style="text-align: center; margin: 10px;">
      <div style="background: #fff3e0; border: 2px solid #ff9800; border-radius: 8px; padding: 15px; min-width: 150px;">
        <div style="font-weight: bold; color: #f57c00; margin-bottom: 10px;">Step 1: Entities</div>
        <div style="font-size: 0.75em; text-align: left; color: #666;">
          • DISH<br>
          • INGREDIENT<br>
          • TECHNIQUE<br>
          • BRAND<br>
          • BEVERAGE<br>
          • PLACE
        </div>
      </div>
    </div>
    <div style="font-size: 24px; color: #2196F3;">→</div>
    <div style="text-align: center; margin: 10px;">
      <div style="background: #f3e5f5; border: 2px solid #9c27b0; border-radius: 8px; padding: 15px; min-width: 150px;">
        <div style="font-weight: bold; color: #7b1fa2; margin-bottom: 10px;">Step 2: Attributes</div>
        <div style="font-size: 0.75em; text-align: left; color: #666;">
          For each entity:<br>
          • Type/Category<br>
          • Characteristics<br>
          • Properties
        </div>
      </div>
    </div>
    <div style="font-size: 24px; color: #2196F3;">→</div>
    <div style="text-align: center; margin: 10px;">
      <div style="background: #e8f5e9; border: 2px solid #4caf50; border-radius: 8px; padding: 15px; min-width: 150px;">
        <div style="font-weight: bold; color: #388e3c; margin-bottom: 10px;">Step 3: Metadata</div>
        <div style="font-size: 0.75em; text-align: left; color: #666;">
          • Cuisine origin<br>
          • Menu language<br>
          • Document type
        </div>
      </div>
    </div>
    <div style="font-size: 24px; color: #2196F3;">→</div>
    <div style="text-align: center; margin: 10px;">
      <div style="background: #e8eaf6; border: 2px solid #3f51b5; border-radius: 8px; padding: 15px; min-width: 150px;">
        <div style="font-weight: bold; color: #303f9f; margin-bottom: 10px;">Annotated Corpus</div>
        <div style="font-size: 0.85em; color: #666;">Final result</div>
      </div>
    </div>
  </div>
  <p style="margin-top: 20px; margin-bottom: 0; font-size: 0.9em; color: #666; font-style: italic;">
    This approach reduces the annotator's cognitive load by dividing the complex task into manageable steps, improving annotation consistency and quality.
  </p>
</div>

**Step 1 - Entity Identification:**
- DISH: Names of complete culinary preparations
- INGREDIENT: Individual recipe components
- TECHNIQUE: Methods and culinary techniques
- BRAND: Commercial product names
- BEVERAGE: Drinks and liquids
- PLACE: Geographic locations related to culinary origin

**Step 2 - Attribute Assignment:**

For each identified entity, specific characteristics are annotated:
- **DISH:** Type (appetizer, main course, side dish, dessert)
- **INGREDIENT:** Category (protein, vegetable, spice, etc.)
- **TECHNIQUE:** Culinary technique classification
- **BRAND:** Product type
- **BEVERAGE:** Classification (alcoholic, non-alcoholic, hot, cold)
- **PLACE:** Cuisine of origin, menu language

**Step 3 - Document Metadata:**
- Menu/recipe cuisine of origin
- Predominant language
- Document type

**Quality control:**

To ensure annotation consistency and quality:
- **Cohen's Kappa (κ):** Target threshold κ ≥ 0.75
- **F1-Score:** Target threshold F1 ≥ 0.85
- **Continuous monitoring:** Annotator overlap for cross-validation
- **Limited sessions:** 1-2 hours per session to mitigate cognitive fatigue
- **Human resources:** 130-150 specialized annotators

**Annotation tool:**

A customized web platform was developed with:
- Intuitive step-guided interface
- Contextual instructions at each phase
- Automatic consistency validations
- Progress tracking system
- Export in standard formats (IOB, JSON)

### 2. Development of Specialized NER Model

**Base architecture:**
- Adaptation of pre-trained models: BERT, SpaCy, Flair
- Fine-tuning with domain-specific annotated corpus

**Training process:**
- Preprocessing to eliminate noise
- Feature extraction (linguistic, orthographic, contextual patterns)
- Implementation of neural networks for entity classification
- Cross-validation

**Evaluation metrics:**
- Precision
- Recall
- F1-score per entity category
- Error analysis by entity type

### 3. Development of Adapted NMT Model

**Base model selection:**
- MarianMT or T5 (pre-trained models for Spanish-English)
- Transformer-based architecture with attention mechanisms

**Domain adaptation:**
- Fine-tuning with bilingual gastronomic corpus
- Optimization for handling specialized terms
- Specific training on gastronomic vocabulary

**Challenges addressed:**
- Out-of-vocabulary (OOV) terms
- Low-frequency terms (exotic ingredients)
- Preservation of proper and culturally relevant names

### 4. NER-NMT Integration

**Integration strategies:**

The innovative proposal consists of modifying the translation pipeline to incorporate NER information in two ways:

<div style="background: linear-gradient(to right, #0f2027, #203a43, #2c5364); padding: 25px; border-radius: 10px; margin: 30px 0; color: white;">
  <h4 style="margin-top: 0; text-align: center; color: white;">Integrated NER-NMT System Architecture</h4>
  <div style="background: rgba(255,255,255,0.1); padding: 20px; border-radius: 8px; margin-top: 20px;">
    <div style="display: flex; flex-direction: column; gap: 15px;">
      <div style="background: #4CAF50; padding: 12px; border-radius: 6px; text-align: center; font-weight: bold;">
        Source Text (Spanish)
      </div>
      <div style="text-align: center; font-size: 20px;">↓</div>
      
      <div style="background: rgba(255,152,0,0.8); padding: 15px; border-radius: 6px; border: 2px solid #ff9800;">
        <div style="font-weight: bold; margin-bottom: 8px;">NER Module</div>
        <div style="font-size: 0.85em; display: grid; grid-template-columns: 1fr 1fr; gap: 8px;">
          <div style="background: rgba(0,0,0,0.2); padding: 6px; border-radius: 4px;">Entity identification</div>
          <div style="background: rgba(0,0,0,0.2); padding: 6px; border-radius: 4px;">IOB tag generation</div>
        </div>
      </div>
      
      <div style="display: flex; justify-content: space-around; align-items: center;">
        <div style="flex: 1; text-align: right; padding-right: 10px; font-size: 0.9em; opacity: 0.8;">IOB Tags</div>
        <div style="font-size: 20px;">↓</div>
        <div style="flex: 1; text-align: left; padding-left: 10px; font-size: 0.9em; opacity: 0.8;">Additional features</div>
      </div>
      
      <div style="background: rgba(33,150,243,0.8); padding: 15px; border-radius: 6px; border: 2px solid #2196F3;">
        <div style="font-weight: bold; margin-bottom: 8px;">NMT Module + NER Features</div>
        <div style="font-size: 0.85em; display: grid; grid-template-columns: 1fr 1fr; gap: 8px;">
          <div style="background: rgba(0,0,0,0.2); padding: 6px; border-radius: 4px;">Neural translation</div>
          <div style="background: rgba(0,0,0,0.2); padding: 6px; border-radius: 4px;">Entity context</div>
        </div>
      </div>
      
      <div style="text-align: center; font-size: 20px;">↓</div>
      
      <div style="background: rgba(156,39,176,0.8); padding: 15px; border-radius: 6px; border: 2px solid #9c27b0;">
        <div style="font-weight: bold; margin-bottom: 8px;">Post-processing</div>
        <div style="font-size: 0.85em; display: grid; grid-template-columns: 1fr 1fr; gap: 8px;">
          <div style="background: rgba(0,0,0,0.2); padding: 6px; border-radius: 4px;">Validation with NER</div>
          <div style="background: rgba(0,0,0,0.2); padding: 6px; border-radius: 4px;">Attention maps</div>
        </div>
      </div>
      
      <div style="text-align: center; font-size: 20px;">↓</div>
      
      <div style="background: #4CAF50; padding: 12px; border-radius: 6px; text-align: center; font-weight: bold;">
        Final Validated Translation (English)
      </div>
    </div>
  </div>
  <p style="margin-top: 20px; margin-bottom: 0; font-size: 0.9em; opacity: 0.9; font-style: italic;">
    The NER model identifies gastronomic entities that are incorporated as features in the NMT. A post-processing module validates and corrects using attention maps, ensuring cultural and semantic coherence.
  </p>
</div>

**A. Preprocessing (Input features):**
- IOB tags generated by NER are incorporated as additional input features to the NMT model
- Improves entity alignment between source and translated text

**B. Post-processing (Entity correction):**
- Use of attention maps to identify discrepancies in entities
- Translation error correction through NER model validation
- Cultural consistency verification

**Implemented techniques:**
- Attention maps for semantic alignment
- Dynamic entity dictionaries
- Cross-validation between NER and NMT

### 5. Integrated System Evaluation

**Automatic metrics:**
- **BLEU:** Evaluation of similarity with human references
- **METEOR:** Consideration of synonyms and variations
- **COMET:** Evaluation based on contextual embeddings

**Human evaluation:**
- Bilingual experts in gastronomy
- Evaluation criteria:
  - Semantic precision
  - Cultural adequacy
  - Translation naturalness
  - Preservation of relevant information

**Comparative design:**
- Integrated NER-NMT system vs. Standard NMT model
- Analysis by text type (menus, recipes, reviews)
- Analysis by entity type

### 6. Error Analysis and Iteration

**Systematic analysis:**
- Categorization of translation errors
- Identification of entity recognition errors
- Analysis of failure patterns
- Identification of improvement areas

**Iterative process:**
- Model adjustment according to results
- Refinement of annotation scheme if necessary
- Hyperparameter optimization
- Continuous improvement of integrated system

## Theoretical Framework

### Named Entity Recognition (NER)

NER is an essential natural language processing task that identifies and classifies specific entities in text. In the gastronomic context, this includes:

- Dish and preparation names
- Ingredients and components
- Culinary techniques
- Commercial brands
- Locations of origin

NER not only allows extracting relevant information but also provides crucial context for specialized terms, significantly improving automatic translation accuracy.

### Neural Machine Translation (NMT)

NMT models based on Transformer architectures have consolidated their position as the dominant technology in automatic translation. These models use attention mechanisms to prioritize relevant parts of source text, improving quality in general contexts.

However, they face challenges in specialized domains where infrequent or out-of-vocabulary terms can generate inaccurate translations. Adaptation through fine-tuning with specialized data has become an essential practice.

### NER-MT Integration

Various studies have explored the integration of NER and MT:

- **IOB tags as features:** Incorporation in the NMT model input to improve alignment
- **Post-processing:** Error correction through attention maps
- **Knowledge transfer:** Adaptation of pre-trained models
- **Annotation projection:** Dataset generation in low-resource languages

### Background in Gastronomic Domain

Previous work has demonstrated the potential of NER in gastronomy:

- **MenuNER:** Entity recognition in restaurant menus
- **SciFood-NER:** Identification in scientific gastronomic texts
- **BuTTER:** Bi-LSTM + CRF model for food entities
- **FoodIE and DrNER:** Rule-based approaches

However, effective integration with automatic translation systems for the Spanish-English pair remains an under-explored area.

## Justification and Relevance

### Cultural Impact

Accurate translation of gastronomic terms allows preserving and promoting cultural heritage. An adequate translation not only describes a dish but also reflects the historical and cultural richness of the communities that prepare it.

### Economic Impact

Gastronomy represents a key economic sector that contributes significantly to employment and global GDP. Accurate translations can help gastronomic businesses reach international markets, strengthening their competitiveness.

### Tourism Impact

The tourism industry depends on clear communication. Accurate translations allow travelers to navigate menus and enjoy authentic culinary experiences without language barriers, significantly improving their experience.

### Technological Advancement

From a technological perspective, the development of this specialized methodology contributes to the advancement of natural language processing, expanding the capabilities of MT systems in specific domains.

### Research Gap

This research fills a gap in current MT system capabilities by:
- Overcoming the scarcity of aligned Spanish-English bilingual resources in gastronomy
- Addressing the limitation of systems that apply NER and MT as separate processes
- Developing an integrated system that ensures proper handling of culturally relevant entities

## Expected Products

### Research Resources

1. **Annotated Bilingual Corpus:** Linguistic resource of 500K+ sentences (Spanish-English) with detailed annotations of gastronomic entities, available to the scientific community as an open research resource.

2. **Annotation Scheme:** Complete documentation of the semantic annotation scheme adapted to the gastronomic domain, replicable for other domains.

### Models and System

3. **Specialized NER Model:** Named entity recognition system optimized for the gastronomic domain with high precision.

4. **Adapted NMT Model:** Neural machine translation system adjusted to gastronomic vocabulary and context.

5. **Integrated Methodology:** Complete experimentally validated, documented, and replicable NER-NMT framework.

6. **Functional Prototype:** Integrated system applicable in real contexts (digital menus, tourism applications).

### Publications

7. **Scientific Article:** Publication in high-impact international conferences (ACL, EMNLP) disseminating research results.

8. **Technical Report:** Detailed documentation including:
   - Complete experimental results
   - Exhaustive error analysis
   - Recommendations for future research
   - Implementation guides

## Practical Applications

### Immediate Applications

- **Intelligent digital menus:** High-quality automatic translation for international restaurants
- **Gastronomic tourist guides:** Information systems for tourists with contextual translation
- **Booking platforms:** Integration in delivery and reservation applications
- **Recommendation systems:** Gastronomic chatbots and virtual assistants

### Future Applications

- **Question answering systems:** QA systems specialized in gastronomy
- **Multilingual review analysis:** Sentiment analysis in gastronomic context
- **Culinary education:** Educational materials translated with cultural precision
- **Heritage documentation:** Digital preservation of culinary traditions

## Limitations and Challenges

### Technical Limitations

1. **Persistent OOV terms:** Some very specific or regional dish names may not have a direct equivalent in the target language.

2. **Complex semantic ambiguity:** Cases where cultural context requires more information than the text provides, requiring human supervision.

3. **Dependency on annotation quality:** System performance critically depends on annotated corpus quality.

4. **Proper name preprocessing:** Risk of losing diacritics and special characters that affect proper name integrity.

### Study Limitations

1. **Linguistic scope:** The study is limited to the Spanish-English pair, although the methodology is extensible to other languages.

2. **Specific domain:** Focused exclusively on gastronomic texts, requiring adaptation for other specialized domains.

3. **Resource cost:** Creating specialized annotated corpora is a costly and laborious process that may limit scalability.

4. **Dialectal variability:** Regional differences in Spanish (Mexican, Argentinian, European, etc.) may affect model generalization.

## Tools and Technologies

### Software and Frameworks

- **Programming language:** Python 3.8+
- **NLP frameworks:** 
  - Hugging Face Transformers
  - SpaCy
  - Flair
- **Deep learning frameworks:**
  - PyTorch
  - TensorFlow
- **Evaluation metrics:**
  - sacreBLEU
  - COMET
  - nltk
- **Data processing:**
  - Pandas
  - NumPy
- **Database:** SQLite
- **Visualization:** Matplotlib, Seaborn
- **Version control:** Git

