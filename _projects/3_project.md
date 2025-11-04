---
layout: page
title: NER-Enhanced Machine Translation for Gastronomic Texts
description: Entity-aware NER-NMT system for culturally accurate Spanish-English translation of gastronomic texts.
img: assets/img/banner-thesis-daniel.png
importance: 3
category: Master's degree
giscus_comments: true
---

# Integrated Methodology for Improving Automatic Translation of Gastronomic Texts through Named Entity Recognition

## General Information

**Principal Investigator:** Daniel Arturo Peña Gnecco

**Director:** Juan Carlos Martinez-Santos

**Co-Director:** Edwin Alexander Puertas del Castillo

**Program:** Master's in Engineering

**Research Line:** Natural Language Processing and Applied Artificial Intelligence

## Abstract

In a globalized world, accurate translation of gastronomic texts is essential for promoting cultural exchange and improving the experience of international users. This research develops an integrated methodology that combines Named Entity Recognition (NER) with Neural Machine Translation (NMT) to optimize translation quality between Spanish and English, preserving the cultural and semantic context of gastronomic texts.

## Problem Description

### Context

Gastronomic texts, including menus, recipes, culinary reviews, and tourist guides, play a crucial role in intercultural communication. However, current automatic translation systems face significant challenges when processing them, especially when they contain culturally specific named entities.

### Core Problem

Neural Machine Translation (NMT) models tend to generate literal translations that omit cultural nuances, lose relevant information, and generate comprehension errors. For example, translating "ceviche" as "raw fish" not only ignores the unique preparation of the dish but can also disorient tourists seeking an authentic culinary experience. Elements such as dish names like mole poblano, ingredients such as chipotle or dashi, and culinary techniques like sous-vide are fundamental for conveying the cultural identity and precise meaning of these texts. The inaccurate translations in menus or reviews hinder communication in international contexts, affecting the experience of non-native users.

### Technical Challenges

The technical challenges are multifaceted and interconnected. First, out-of-vocabulary (OOV) terms, particularly exotic ingredients and traditional dish names, often generate inaccurate translations due to their low frequency in training data. Second, semantic ambiguity persists because cultural context is crucial for adequate translation, yet conventional systems prioritize literal translations. Third, there is a notable scarcity of bilingual resources, as the absence of specialized annotated corpora in the gastronomic domain for the Spanish-English pair limits the training of adapted models. Finally, current systems apply NER and MT as independent processes, preventing exploitation of synergies between entity identification and culturally informed translation.

<div style="background: #ffffff; border: 2px solid #333; padding: 30px; margin: 40px 0; font-family: 'Times New Roman', serif;">
  <h4 style="text-align: center; font-weight: normal; font-size: 1.1em; margin: 0 0 25px 0; color: #333; border-bottom: 1px solid #333; padding-bottom: 10px;">Figure 1: Comparison of Translation Approaches</h4>
  
  <table style="width: 100%; border-collapse: collapse; background: white;">
    <thead>
      <tr style="border-bottom: 2px solid #333;">
        <th style="padding: 12px; text-align: left; font-weight: normal; width: 50%; border-right: 1px solid #ddd;">Traditional NMT System</th>
        <th style="padding: 12px; text-align: left; font-weight: normal; width: 50%;">Proposed Integrated System</th>
      </tr>
    </thead>
    <tbody>
      <tr>
        <td style="padding: 15px; vertical-align: top; border-right: 1px solid #ddd;">
          <div style="background: #f9f9f9; padding: 12px; margin-bottom: 12px; border-left: 3px solid #999; font-family: monospace; font-size: 0.9em;">
            Input: "Ceviche de pescado"<br>
            Process: Direct NMT<br>
            Output: "Raw fish ceviche"
          </div>
          <p style="margin: 0; font-size: 0.9em; line-height: 1.6; color: #555;">
            <strong>Limitations:</strong> The system produces literal translations without cultural context. Entity recognition is absent, resulting in loss of semantic meaning and cultural significance. No preprocessing identifies culturally relevant terms.
          </p>
        </td>
        <td style="padding: 15px; vertical-align: top;">
          <div style="background: #f9f9f9; padding: 12px; margin-bottom: 12px; border-left: 3px solid #333; font-family: monospace; font-size: 0.9em;">
            Input: "Ceviche de pescado"<br>
            Process: NER → Entity tagging → NMT<br>
            Output: "Peruvian ceviche"
          </div>
          <p style="margin: 0; font-size: 0.9em; line-height: 1.6; color: #555;">
            <strong>Advantages:</strong> The integrated approach identifies entities before translation, enabling culturally informed decisions. Context preservation maintains semantic integrity while entity-aware translation produces culturally appropriate output.
          </p>
        </td>
      </tr>
    </tbody>
  </table>
  
  <p style="margin-top: 20px; font-size: 0.85em; color: #666; line-height: 1.5; text-align: justify;">
    <em>Note:</em> The traditional approach fails to recognize "ceviche" as a culturally significant dish entity, resulting in literal translation. The proposed system first identifies the entity type (DISH) and cultural origin, then applies context-aware translation that preserves the cultural meaning.
  </p>
</div>

### Research Question

How can the integration of Named Entity Recognition (NER) in neural machine translation (NMT) systems improve the quality of gastronomic text translations between Spanish and English, ensuring the preservation of cultural and semantic context?

## Objectives

### General Objective

Design and evaluate an integrated methodology that combines Named Entity Recognition (NER) with Neural Machine Translation (NMT) to improve the quality of gastronomic text translations between Spanish and English, preserving cultural and semantic context.

### Specific Objectives

The research pursues four specific objectives. First, it aims to create a bilingual corpus (Spanish-English) of gastronomic texts annotated with named entities, including dish names, ingredients, and culinary techniques, with proper categorization to lay the foundation for developing specialized models. Second, the study will develop a specialized NER model for the gastronomic domain, trained with the bilingual corpus and capable of recognizing entities with high precision to support contextualized translation. Third, it seeks to create a Neural Machine Translation (NMT) model adapted to the gastronomic domain through fine-tuning, integrating the NER model to ensure proper handling of named entities. Finally, the research will evaluate the integrated system using automatic metrics such as BLEU and METEOR, complemented by human evaluations focusing on precision and cultural adequacy.

## Proposed Methodology

The research adopts a quantitative and experimental approach with a comparative design that seeks to evaluate the effectiveness of integrating NER and NMT in gastronomic translation. The methodology consists of six interconnected phases that build upon each other to create a comprehensive translation system.

### 1. Collection and Annotation of Bilingual Corpus

The corpus construction targets 517,088 balanced sentences between recipes and menus, drawing from diverse data sources including restaurant menus, culinary recipes, gastronomic reviews, and gastronomic tourist guides. This diversity ensures comprehensive coverage of gastronomic language variations and contexts.

The annotation strategy follows a sequential two-step process that balances semantic richness with low cognitive load. This approach was specifically designed to reduce annotator fatigue while maintaining high-quality annotations. The process begins with entity identification, proceeds to attribute assignment, and concludes with metadata documentation.

<div style="background: #ffffff; border: 2px solid #333; padding: 30px; margin: 40px 0; font-family: 'Times New Roman', serif;">
  <h4 style="text-align: center; font-weight: normal; font-size: 1.1em; margin: 0 0 25px 0; color: #333; border-bottom: 1px solid #333; padding-bottom: 10px;">Figure 2: Sequential Annotation Methodology</h4>
  
  <div style="display: flex; flex-direction: column; gap: 20px;">
    <div style="display: grid; grid-template-columns: repeat(5, 1fr); gap: 15px; align-items: center;">
      <div style="background: #f5f5f5; border: 1px solid #333; padding: 15px; text-align: center;">
        <div style="font-weight: bold; color: #333; margin-bottom: 8px; font-size: 0.9em;">Raw Text</div>
        <div style="font-size: 0.75em; color: #666;">Input</div>
      </div>
      
      <div style="text-align: center; font-size: 1.5em; color: #333;">→</div>
      
      <div style="background: #f5f5f5; border: 1px solid #333; padding: 15px; text-align: center;">
        <div style="font-weight: bold; color: #333; margin-bottom: 8px; font-size: 0.9em;">Step 1</div>
        <div style="font-size: 0.75em; color: #666;">Entity<br>Identification</div>
      </div>
      
      <div style="text-align: center; font-size: 1.5em; color: #333;">→</div>
      
      <div style="background: #f5f5f5; border: 1px solid #333; padding: 15px; text-align: center;">
        <div style="font-weight: bold; color: #333; margin-bottom: 8px; font-size: 0.9em;">Step 2</div>
        <div style="font-size: 0.75em; color: #666;">Attribute<br>Assignment</div>
      </div>
    </div>
    
    <div style="display: grid; grid-template-columns: repeat(3, 1fr); gap: 15px; align-items: center; justify-items: center;">
      <div></div>
      
      <div style="text-align: center; font-size: 1.5em; color: #333;">→</div>
      
      <div></div>
    </div>
    
    <div style="display: grid; grid-template-columns: repeat(3, 1fr); gap: 15px; align-items: center;">
      <div></div>
      
      <div style="background: #f5f5f5; border: 1px solid #333; padding: 15px; text-align: center;">
        <div style="font-weight: bold; color: #333; margin-bottom: 8px; font-size: 0.9em;">Step 3</div>
        <div style="font-size: 0.75em; color: #666;">Metadata<br>Documentation</div>
      </div>
      
      <div></div>
    </div>
    
    <div style="display: grid; grid-template-columns: repeat(3, 1fr); gap: 15px; align-items: center; justify-items: center;">
      <div></div>
      
      <div style="text-align: center; font-size: 1.5em; color: #333;">↓</div>
      
      <div></div>
    </div>
    
    <div style="display: grid; grid-template-columns: repeat(3, 1fr); gap: 15px; align-items: center;">
      <div></div>
      
      <div style="background: #e8e8e8; border: 2px solid #333; padding: 15px; text-align: center;">
        <div style="font-weight: bold; color: #333; font-size: 0.9em;">Annotated Corpus</div>
      </div>
      
      <div></div>
    </div>
  </div>
  
  <table style="width: 100%; margin-top: 25px; border-collapse: collapse; font-size: 0.85em;">
    <thead>
      <tr style="border-bottom: 2px solid #333;">
        <th style="padding: 10px; text-align: left; font-weight: normal;">Phase</th>
        <th style="padding: 10px; text-align: left; font-weight: normal;">Description</th>
        <th style="padding: 10px; text-align: left; font-weight: normal;">Output</th>
      </tr>
    </thead>
    <tbody>
      <tr style="border-bottom: 1px solid #ddd;">
        <td style="padding: 10px;">Step 1</td>
        <td style="padding: 10px;">Identification of entity types (DISH, INGREDIENT, TECHNIQUE, BRAND, BEVERAGE, PLACE)</td>
        <td style="padding: 10px;">Tagged entities</td>
      </tr>
      <tr style="border-bottom: 1px solid #ddd;">
        <td style="padding: 10px;">Step 2</td>
        <td style="padding: 10px;">Assignment of specific attributes and characteristics to each identified entity</td>
        <td style="padding: 10px;">Detailed annotations</td>
      </tr>
      <tr>
        <td style="padding: 10px;">Step 3</td>
        <td style="padding: 10px;">Documentation of document-level metadata (cuisine origin, language, type)</td>
        <td style="padding: 10px;">Complete corpus</td>
      </tr>
    </tbody>
  </table>
  
  <p style="margin-top: 20px; font-size: 0.85em; color: #666; line-height: 1.5; text-align: justify;">
    <em>Note:</em> This sequential approach reduces cognitive load by separating the complex annotation task into manageable stages, improving consistency and quality while maintaining annotator efficiency across extended annotation sessions.
  </p>
</div>

In the first step of entity identification, annotators identify six primary entity types. DISH entities represent names of complete culinary preparations. INGREDIENT entities capture individual recipe components. TECHNIQUE entities encompass methods and culinary techniques. BRAND entities identify commercial product names. BEVERAGE entities include drinks and liquids. Finally, PLACE entities represent geographic locations related to culinary origin. This categorization provides a comprehensive framework for capturing the essential elements of gastronomic texts.

The second step involves attribute assignment, where each identified entity receives specific characteristic annotations. For DISH entities, the type is specified as appetizer, main course, side dish, or dessert. INGREDIENT entities are categorized by type such as protein, vegetable, or spice. TECHNIQUE entities receive classification according to culinary technique types. BRAND entities are annotated with product type information. BEVERAGE entities are classified as alcoholic, non-alcoholic, hot, or cold. PLACE entities include annotations for cuisine of origin and menu language. This detailed attribute assignment enables fine-grained analysis and translation decisions.

The third step focuses on document metadata, capturing cuisine of origin for the menu or recipe, predominant language, and document type. This contextual information provides essential background for understanding the cultural framework of the text.

Quality control mechanisms ensure annotation consistency and reliability. Cohen's Kappa coefficient (κ) targets a threshold of κ ≥ 0.75, while F1-Score aims for F1 ≥ 0.85. Continuous monitoring through annotator overlap enables cross-validation. Sessions are limited to one to two hours to mitigate cognitive fatigue. The project employs 130-150 specialized annotators to complete the corpus annotation within the planned timeframe.

A customized web platform supports the annotation process with an intuitive step-guided interface, contextual instructions at each phase, automatic consistency validations, progress tracking system, and export capabilities in standard formats including IOB and JSON.

### 2. Development of Specialized NER Model

The NER model development adapts pre-trained models including BERT, SpaCy, and Flair through fine-tuning with the domain-specific annotated corpus. The training process begins with preprocessing to eliminate noise, followed by feature extraction focusing on linguistic, orthographic, and contextual patterns. Neural networks are implemented for entity classification, and cross-validation ensures robust model performance.

Evaluation employs multiple metrics to assess model quality comprehensively. Precision measures the accuracy of positive predictions. Recall assesses the model's ability to identify all relevant entities. F1-score provides a balanced measure combining precision and recall. Additionally, detailed error analysis by entity type identifies specific areas requiring improvement and informs iterative model refinement.

### 3. Development of Adapted NMT Model

Model selection focuses on established pre-trained models for Spanish-English translation, particularly MarianMT and T5, which employ Transformer-based architectures with attention mechanisms. These models provide a strong foundation for domain adaptation.

Domain adaptation proceeds through fine-tuning with the bilingual gastronomic corpus, optimizing the model for handling specialized terms and training specifically on gastronomic vocabulary. This process addresses several key challenges. First, it tackles out-of-vocabulary (OOV) terms that frequently appear in gastronomic texts. Second, it handles low-frequency terms such as exotic ingredients that standard models struggle with. Third, it ensures preservation of proper names and culturally relevant terms that are essential for maintaining translation quality in this domain.

### 4. NER-NMT Integration

The innovative integration strategy modifies the translation pipeline to incorporate NER information through two complementary approaches. The preprocessing approach incorporates IOB tags generated by NER as additional input features to the NMT model, improving entity alignment between source and translated text. The post-processing approach employs attention maps to identify discrepancies in entities, corrects translation errors through NER model validation, and verifies cultural consistency.

<div style="background: #ffffff; border: 2px solid #333; padding: 30px; margin: 40px 0; font-family: 'Times New Roman', serif;">
  <h4 style="text-align: center; font-weight: normal; font-size: 1.1em; margin: 0 0 25px 0; color: #333; border-bottom: 1px solid #333; padding-bottom: 10px;">Figure 3: Integrated NER-NMT System Architecture</h4>
  
  <div style="border: 1px solid #666; background: #fafafa;">
    <table style="width: 100%; border-collapse: collapse;">
      <tr style="border-bottom: 1px solid #666;">
        <td style="padding: 15px; text-align: center; background: #e8e8e8; font-weight: bold;">
          Input Layer
        </td>
      </tr>
      <tr style="border-bottom: 1px solid #666;">
        <td style="padding: 12px; text-align: center; background: #f5f5f5;">
          Source Text (Spanish)
        </td>
      </tr>
      <tr style="border-bottom: 1px solid #666;">
        <td style="padding: 20px; text-align: center;">
          ↓
        </td>
      </tr>
      <tr style="border-bottom: 1px solid #666;">
        <td style="padding: 15px; background: #f9f9f9;">
          <div style="border-left: 3px solid #666; padding-left: 15px;">
            <strong>Module 1: Named Entity Recognition</strong>
            <div style="margin-top: 10px; font-size: 0.9em; color: #555;">
              Function: Entity identification and classification<br>
              Output: IOB-tagged entities with type annotations
            </div>
          </div>
        </td>
      </tr>
      <tr style="border-bottom: 1px solid #666;">
        <td style="padding: 20px; text-align: center;">
          ↓<br>
          <span style="font-size: 0.85em; color: #666;">[Entity features + IOB tags]</span>
        </td>
      </tr>
      <tr style="border-bottom: 1px solid #666;">
        <td style="padding: 15px; background: #f9f9f9;">
          <div style="border-left: 3px solid #666; padding-left: 15px;">
            <strong>Module 2: Neural Machine Translation</strong>
            <div style="margin-top: 10px; font-size: 0.9em; color: #555;">
              Function: Context-aware translation with entity features<br>
              Process: Transformer-based translation with attention to entity tags
            </div>
          </div>
        </td>
      </tr>
      <tr style="border-bottom: 1px solid #666;">
        <td style="padding: 20px; text-align: center;">
          ↓<br>
          <span style="font-size: 0.85em; color: #666;">[Preliminary translation]</span>
        </td>
      </tr>
      <tr style="border-bottom: 1px solid #666;">
        <td style="padding: 15px; background: #f9f9f9;">
          <div style="border-left: 3px solid #666; padding-left: 15px;">
            <strong>Module 3: Post-processing and Validation</strong>
            <div style="margin-top: 10px; font-size: 0.9em; color: #555;">
              Function: Entity validation and cultural consistency verification<br>
              Method: Attention map analysis and NER-based correction
            </div>
          </div>
        </td>
      </tr>
      <tr style="border-bottom: 1px solid #666;">
        <td style="padding: 20px; text-align: center;">
          ↓
        </td>
      </tr>
      <tr style="border-bottom: 1px solid #666;">
        <td style="padding: 12px; text-align: center; background: #f5f5f5;">
          Final Validated Translation (English)
        </td>
      </tr>
      <tr>
        <td style="padding: 15px; text-align: center; background: #e8e8e8; font-weight: bold;">
          Output Layer
        </td>
      </tr>
    </table>
  </div>
  
  <p style="margin-top: 20px; font-size: 0.85em; color: #666; line-height: 1.5; text-align: justify;">
    <em>Note:</em> The architecture implements a three-stage pipeline where NER preprocessing informs the translation process, and post-processing validation ensures entity coherence. This integration enables culturally and semantically accurate translations by maintaining entity awareness throughout the translation pipeline.
  </p>
</div>

The implementation employs several sophisticated techniques. Attention maps enable semantic alignment between source and target entities. Dynamic entity dictionaries provide reference information for culturally significant terms. Cross-validation between NER and NMT modules ensures consistency and catches potential translation errors before final output.

### 5. Integrated System Evaluation

The evaluation framework combines automatic metrics with human assessment to provide comprehensive quality measurement. Automatic metrics include BLEU for evaluating similarity with human references, METEOR for considering synonyms and variations, and COMET for evaluation based on contextual embeddings. These metrics provide quantitative measures of translation quality that enable systematic comparison.

Human evaluation involves bilingual experts in gastronomy who assess translations according to multiple criteria. Semantic precision measures whether the translation accurately conveys the original meaning. Cultural adequacy evaluates whether culturally specific elements are appropriately handled. Translation naturalness assesses whether the output reads fluently in the target language. Preservation of relevant information verifies that no critical details are lost in translation.

The comparative design contrasts the integrated NER-NMT system against a standard NMT model baseline. Analysis proceeds along two dimensions: by text type, examining performance on menus, recipes, and reviews separately; and by entity type, assessing how well different categories of entities are handled. This multifaceted evaluation reveals the specific strengths and weaknesses of the integrated approach.

### 6. Error Analysis and Iteration

Systematic error analysis categorizes translation errors, identifies entity recognition failures, analyzes failure patterns, and pinpoints specific areas requiring improvement. This analysis feeds into an iterative refinement process.

The iterative process involves multiple cycles of improvement. Models are adjusted according to evaluation results. The annotation scheme is refined if systematic issues are identified. Hyperparameters are optimized to improve performance. Through continuous improvement cycles, the integrated system evolves toward higher quality and reliability.

## Theoretical Framework

### Named Entity Recognition (NER)

NER constitutes an essential natural language processing task that identifies and classifies specific entities in text. In the gastronomic context, this encompasses dish and preparation names, ingredients and components, culinary techniques, commercial brands, and locations of origin. Beyond simple information extraction, NER provides crucial context for specialized terms, significantly improving automatic translation accuracy by identifying which elements require special handling during the translation process.

### Neural Machine Translation (NMT)

NMT models based on Transformer architectures have consolidated their position as the dominant technology in automatic translation. These models employ attention mechanisms to prioritize relevant parts of source text, substantially improving quality in general contexts. However, they face notable challenges in specialized domains where infrequent or out-of-vocabulary terms can generate inaccurate translations. Consequently, adaptation through fine-tuning with specialized data has become an essential practice for domain-specific translation tasks, including gastronomic text translation.

### NER-MT Integration

Various studies have explored the integration of NER and MT through different approaches. IOB tags can be incorporated as features in the NMT model input to improve alignment. Post-processing enables error correction through attention maps. Knowledge transfer facilitates adaptation of pre-trained models. Annotation projection supports dataset generation in low-resource languages. These approaches demonstrate the potential benefits of combining entity recognition with translation, though effective integration for Spanish-English gastronomic translation remains under-explored.

### Background in Gastronomic Domain

Previous work has demonstrated NER's potential in gastronomy through several notable systems. MenuNER performs entity recognition in restaurant menus. SciFood-NER identifies entities in scientific gastronomic texts. BuTTER implements a Bi-LSTM plus CRF model for food entities. FoodIE and DrNER employ rule-based approaches. However, effective integration with automatic translation systems for the Spanish-English pair remains an under-explored area, representing a significant research opportunity that this work addresses.

## Justification and Relevance

### Cultural Impact

Accurate translation of gastronomic terms enables preservation and promotion of cultural heritage. An adequate translation not only describes a dish but also reflects the historical and cultural richness of the communities that prepare it, maintaining connections to culinary traditions and fostering cross-cultural understanding.

### Economic Impact

Gastronomy represents a key economic sector that contributes significantly to employment and global GDP. Accurate translations can help gastronomic businesses reach international markets, strengthening their competitiveness and enabling economic growth through improved communication with international customers and partners.

### Tourism Impact

The tourism industry depends fundamentally on clear communication. Accurate translations allow travelers to navigate menus and enjoy authentic culinary experiences without language barriers, significantly improving their experience and potentially increasing tourism revenue for destinations with strong gastronomic offerings.

### Technological Advancement

From a technological perspective, the development of this specialized methodology contributes to the advancement of natural language processing by expanding the capabilities of MT systems in specific domains. The techniques and resources developed can potentially transfer to other specialized translation domains beyond gastronomy.

### Research Gap

This research fills a significant gap in current MT system capabilities through three main contributions. First, it overcomes the scarcity of aligned Spanish-English bilingual resources in gastronomy by creating a substantial annotated corpus. Second, it addresses the limitation of systems that apply NER and MT as separate processes by developing truly integrated approaches. Third, it develops an integrated system that ensures proper handling of culturally relevant entities, advancing the state of the art in domain-specific translation.

## Expected Products

### Research Resources

The research will produce an annotated bilingual corpus comprising over 500,000 sentences in Spanish and English with detailed annotations of gastronomic entities, available to the scientific community as an open research resource. Additionally, complete documentation of the semantic annotation scheme adapted to the gastronomic domain will be provided, designed to be replicable for other domains and serving as a methodological reference for similar annotation projects.

### Models and System

The project will deliver a specialized NER model optimized for the gastronomic domain with high precision in entity recognition. An adapted NMT model will be developed, specifically adjusted to gastronomic vocabulary and context. The complete experimentally validated NER-NMT framework will be fully documented and designed for replicability. A functional prototype will demonstrate the integrated system's applicability in real contexts such as digital menus and tourism applications.


