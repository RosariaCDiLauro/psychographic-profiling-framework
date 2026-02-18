# 🧠 Psychographic Cyber Targeting
*A Computational Framework for Psychographic Profiling in Digital Environments*

**Author:** Rosaria Chiara Di Lauro

*[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/RosariaCDiLauro/psychographic-profiling-experiment/blob/main/psychographic-profiling-experiment.ipynb)*

---

## 📑 Table of Contents
1. [Project Overview](#project-overview)  
2. [Scientific Context](#scientific-context)  
3. [Research Objective](#research-objective)  
4. [Dataset and Data Source](#dataset-and-data-source)  
5. [System Architecture](#system-architecture)  
6. [Psychographic Dimensions](#psychographic-dimensions)  
7. [Vulnerability Modeling](#vulnerability-modeling)  
8. [Contextual (Subreddit) Analysis](#contextual-subreddit-analysis)  
9. [Output and Interpretation](#output-and-interpretation)  
10. [Reproducibility and Scientific Use](#reproducibility-and-scientific-use)  
11. [Ethical and Methodological Note](#ethical-and-methodological-note)  
12. [License](#license)

---

## Project Overview

This repository contains a **computational framework for psychographic profiling** designed to analyze how emotional patterns, personality traits, and discursive environments interact to produce **cognitive and affective configurations** in digital users.

The system processes large-scale social media data (Reddit posts and comments) and extracts:

- Emotional distributions  
- Big-Five personality traits (OCEAN model)  
- Dominant discussion environments  
- Group-level psychographic configurations  

The final goal is to model how **psychological profiling frameworks can be theoretically applied within cyber targeting and influence research contexts**, as explored in the associated master’s thesis:

> **“Psychographic Profiling: The Role of Psychology in Understanding Cyber Targeting Processes”**

---

## Scientific Context

Modern cyber operations increasingly involve **psychological and informational dynamics** rather than purely technical exploits.  
Influence campaigns, disinformation, and psychological operations (PSYOPs) have been studied as processes that leverage **differential cognitive and emotional predispositions** to persuasion.

This project integrates three scientific domains:

- **Computational social science**  
- **Personality psychology (OCEAN / Big Five)**  
- **Emotion analysis (multi-label affective classification)**  

into a single pipeline that allows **data-driven psychographic modeling at scale**.

---


## Research Objective

The core objective is to answer the following research question:

> *Can computational models combining emotions, personality traits, and discursive context identify differential susceptibility to persuasive and influence dynamics in online environments?*

Rather than focusing on individual users, the system operates on **clusters and groups**, identifying **psychographic configurations** that exhibit differential responsiveness to persuasion and narrative framing processes.

---


## Dataset and Data Source

The framework operates on Reddit data structured in tabular format.  
Each row represents a user-generated contribution containing the following attributes:

- Author  
- Subreddit (context)  
- Text content  
- Predicted emotions (multi-label classification)  
- Predicted personality traits (OCEAN scores)

The raw textual data originates from Reddit, while emotional and personality features are inferred through computational models.

Emotional signals are derived using a combination of:

- Models trained on **GoEmotions** (fine-grained multi-label affect taxonomy)  
- The **NRC Emotion Lexicon (EmoLex)** for lexicon-based affective mapping  
- **VADER sentiment analysis** for polarity and intensity scoring  

Personality traits are inferred following the **Big Five model**, leveraging computational personality prediction approaches and reference datasets such as **PANDORA**.

The five personality dimensions considered are:

- Openness  
- Conscientiousness  
- Extraversion  
- Agreeableness  
- Neuroticism  

---

## System Architecture

The pipeline implemented in the notebook follows these stages:

1. **Data loading and preprocessing**  
2. **Emotion normalization and aggregation**  
3. **Personality trait aggregation at user and group level**  
4. **Subreddit (context) extraction**  
5. **Psychographic cluster computation**  
6. **Susceptibility modeling**  
7. **Interpretation and reporting**

Each step transforms raw textual signals into **structured psychological indicators** that support analytical reasoning about influence exposure dynamics in digital environments.

---

## Psychographic Dimensions

Two primary dimensions are extracted:

### Emotional Structure
The model computes:
- Dominant emotions  
- Emotional volatility  
- Conflict-oriented vs regulation-oriented affective patterns  

### Personality Structure
Based on OCEAN:
- Trait distributions are analyzed at group level  
- Personality configurations are examined in relation to emotional and contextual patterns  

These dimensions are combined to build **psychographic configurations** of groups.

---

## Susceptibility Modeling

Susceptibility is not defined as a single variable but as a **multidimensional construct** emerging from:

- Elevated emotional reactivity  
- Conflict-oriented or negatively valenced emotional clusters  
- Personality configurations observed in relation to emotional and contextual dynamics  

The framework computes a **composite susceptibility score** for each group by integrating these components.

This score represents **differential responsiveness to persuasive and narrative dynamics** within digital environments.

---

## Contextual (Subreddit) Analysis

The system extracts the dominant subreddits associated with each group, allowing the identification of:

- Generalist vs niche communities  
- Political, social, or identity-based spaces  
- Emotional climates of different discursive environments  

Importantly, the system highlights that **susceptibility patterns are not determined by the platform itself**, but emerge from the interaction between:

> personality × emotion × context

---

## Output and Interpretation

The notebook produces:

- Group-level emotional profiles  
- Personality trait distributions  
- Dominant discussion environments  
- Composite susceptibility indices  
- Interpretative summaries  

These outputs allow researchers to reason about **how different psychographic configurations may respond to influence dynamics in digital contexts**.

---

## Reproducibility and Scientific Use

This project is designed as a **reproducible experimental framework**.

The notebook:
- Can be rerun on any compatible dataset  
- Produces transparent intermediate outputs  
- Supports comparative group analysis  

This makes it suitable for:
- Academic replication  
- Methodological validation  
- Extension to other platforms or datasets  

---

## Ethical and Methodological Note

The dataset used does **not** originate from real military or intelligence operations.  
It represents **open, civilian online discourse**.

Therefore:
- The framework demonstrates **methodological feasibility**
- Not operational deployment  

The project is intended exclusively for academic research on influence dynamics and psychographic modeling.

The goal is to examine how such analytical approaches **can contribute to understanding influence processes**, not to operationalize targeting practices.

---

## License

This project is released under the **MIT License**, allowing free use, modification, and academic or industrial application with proper attribution.  
See the [LICENSE](LICENSE) file for full terms and conditions.
