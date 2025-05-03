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

## Natural Language Processing

![NLP Banner](https://api.placeholder.com/1200/300)

---

### Descripción del curso

| **Instructor**           | Edwin Puertas, PhD.                           | **Correo electrónico**     | epuerta@utb.edu.co                       |
|--------------------------|-----------------------------------------------|----------------------------|------------------------------------------|
| **Oficina**              | AL-304                                        | **Facultad**               | School of Digital Transformation         |
| **Horas semanales**      | 3                                             | **Créditos**               | 4                                        |
| **Modalidad**            | Presencial                                    | **Metodología**            | Sesiones teóricas                        |

---

### Objetivo general

Desarrollar competencias teóricas y prácticas en Procesamiento de Lenguaje Natural (PLN), que permitan aplicar técnicas y modelos de aprendizaje automático para analizar, comprender y generar texto en diversos contextos, con un enfoque ético y sostenible.

#### Objetivos específicos

1. Comprender los fundamentos teóricos del PLN, incluyendo modelos de lenguaje, análisis de sentimiento, semántica vectorial y redes neuronales.  
2. Implementar modelos supervisados y no supervisados con Python, NLTK y TensorFlow.  
3. Evaluar y optimizar modelos de PLN mediante métricas adecuadas y ajuste de hiperparámetros.  
4. Desarrollar proyectos de PLN en equipo, fortaleciendo habilidades de comunicación, colaboración y pensamiento crítico.  

---

### Metodología

El proceso de aprendizaje se articula en cuatro tipos de actividades complementarias:

- **Exposiciones temáticas**  
  Presentaciones por parte del docente, complementadas con discusiones y aportes de los estudiantes.

- **Tareas individuales**  
  Ejercicios prácticos para validar la comprensión y preparación de los contenidos.

- **Talleres grupales**  
  Desarrollo colaborativo de conceptos y técnicas mediante casos prácticos.

- **Evaluaciones**  
  Pruebas individuales para medir el avance de los estudiantes.

---

### Temario

| **Módulo 1: Fundamentos de PLN**           | **Módulo 2: Aprendizaje automático y PLN**     | **Módulo 3: Aplicaciones y ética**                           |
|--------------------------------------------|-----------------------------------------------|--------------------------------------------------------------|
| 1. Introducción al PLN                     | 1. Redes neuronales y modelos de lenguaje     | 1. Traducción automática y generación de texto               |
| 2. Expresiones regulares y normalización   | 2. Etiquetado de secuencias (POS, entidades)  | 2. Recuperación de información y sistemas de pregunta–respuesta |
| 3. Modelos de lenguaje N-gram              | 3. RNN, LSTM y modelos avanzados              | 3. Desarrollo de chatbots y sistemas de diálogo              |
| 4. Clasificación de texto y análisis de sentimiento | 4. Transformers y modelos de gran escala (BERT, GPT) | 4. Reconocimiento de voz y síntesis de voz                   |
| 5. Regresión logística y semántica vectorial | 5. Ajuste fino, prompting y aprendizaje en contexto | 5. Consideraciones éticas y reducción de desigualdades      |

---

### Bibliografía

- Jurafsky, D. & Martin, J. H. (2020). *Speech and Language Processing* (3rd ed. draft).  
- Beysolow II, T. (2018). *Applied Natural Language Processing with Python*. Apress.  
- Vajjala, S., Majumder, B., Gupta, A. & Surana, H. (2020). *Practical Natural Language Processing*. O’Reilly Media.  
- Srinivasa-Desikan, B. (2018). *Natural Language Processing and Computational Linguistics*. Packt Publishing.

---

## Introducción al PLN

**Procesamiento de Lenguaje Natural (PLN)** estudia tanto los aspectos teóricos como prácticos en el diseño e implementación de sistemas informáticos para el tratamiento de lenguajes humanos.

---

## Niveles de análisis lingüístico

| Nivel       | Descripción                                                                         |
|-------------|-------------------------------------------------------------------------------------|
| Fonética    | Estudio de los sonidos del habla: producción, transmisión y percepción.             |
| Fonología   | Análisis de los sistemas de sonidos y su función en una lengua determinada.         |
| Morfología  | Examen de la formación de palabras y sus unidades mínimas de significado (morfemas).|
| Sintaxis    | Estructura de las oraciones y organización de palabras y frases.                    |
| Semántica   | Estudio del significado en palabras y oraciones, tanto léxico como composicional.   |
| Pragmática  | Uso del lenguaje en contexto social, intenciones del hablante e implicaciones.      |

---

## Componentes clave del PLN

| Componente                      | Descripción                                                   |
|---------------------------------|---------------------------------------------------------------|
| Preprocesamiento de texto       | Transformación del texto bruto en un formato legible por máquinas. |
| Extracción de características   | Conversión de texto a representaciones numéricas.             |
| POS tagging                     | Identificación de la función gramatical de cada palabra.      |
| Reconocimiento de entidades     | Detección de nombres, lugares y fechas relevantes.            |
| Resolución de correferencias    | Identificación de referencias a la misma entidad.             |
| Análisis sintáctico             | Estructuración gramatical para extraer significado.           |

---

## Técnicas y algoritmos fundamentales

- **Tokenización:** División del texto en unidades mínimas.  
- **Lematización / Stemizado:** Reducción de palabras a su forma raíz.  
- **Parsing de dependencias:** Identificación de relaciones sintácticas.  
- **Bag of Words / TF-IDF:** Representaciones basadas en frecuencia y peso de términos.  
- **Word Embeddings:** Vectores que capturan similitud semántica.  
- **Modelos preentrenados:** Redes entrenadas en grandes corpus de texto.  

---

## Aplicaciones prácticas

1. **Análisis de sentimiento**  
2. **Sistemas de diálogo y chatbots**  
3. **Traducción automática**  
4. **Extracción de información**  
5. **Generación automática de texto**  
