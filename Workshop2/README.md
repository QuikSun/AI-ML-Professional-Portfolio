# Workshop 2 — Machine Learning vs. Deep Learning

## Overview

This workshop explores the differences between traditional machine learning (ML) and deep learning (DL), focusing on their applications, capabilities, limitations, and suitability for different analytical problems.

The central research question is:

**How should organizations choose between traditional machine learning and deep learning when solving real-world problems?**

Using two case studies—**customer churn prediction** and **machine translation**—this project examines how data structure, model complexity, computational requirements, and interpretability influence algorithm selection.

The central conclusion is that **model suitability matters more than model complexity**. More sophisticated algorithms do not necessarily produce better solutions for every problem.

## Project Components

### 1. Research Paper — Machine Learning vs. Deep Learning

The academic paper examines two applications:

**Customer Churn Prediction — Traditional Machine Learning**

Explores supervised classification using Support Vector Machines (SVMs), with consideration of alternative approaches such as Random Forest and Gradient Boosting. The research evaluates why traditional ML methods can provide effective solutions for structured customer data.

**Machine Translation — Deep Learning**

Examines Transformer-based neural networks and their ability to learn contextual relationships within language sequences. The research discusses why deep learning architectures are well suited to complex natural language processing tasks.

The paper also evaluates trade-offs in data requirements, computational resources, interpretability, and predictive performance.

**Artifact:** [View Research Paper](./Assignment-2.3/)

### 2. Infographic — Choosing the Right Approach

A professional visual summary of the research, designed to make technical concepts accessible to business analysts, employers, and readers without extensive machine learning experience.

The infographic highlights:

- Differences between traditional ML and DL.
- Customer churn prediction versus machine translation.
- Model capabilities and practical limitations.
- A five-step framework for selecting an appropriate analytical approach.
- The importance of evidence-based model evaluation.

**Artifact:** [View Infographic](./Infographic/)

### 3. Interactive Simulation — Customer Churn Classifier

This interactive simulation demonstrates the conceptual workflow of a supervised machine learning classifier used to predict customer churn.

Visitors can explore how customer characteristics, such as service usage, tenure, and engagement, influence simulated churn-risk classifications.

**Concepts Demonstrated:**
- Structured data and input features
- Supervised classification
- Customer churn risk assessment
- Interpreting classification outputs
- Business applications of predictive analytics

**Purpose:** Help visitors understand how customer data can inform retention decisions through classification-based analysis.

**Important:** This is an educational simulation, not a trained or validated SVM model. The outputs are illustrative and should not be interpreted as actual predictions.

### 4. Interactive Simulation — Deep Learning Translator

This interactive simulation demonstrates the conceptual workflow of neural machine translation using Transformer-based deep learning.

Visitors can explore how input text is processed conceptually to produce a translated output, illustrating the role of contextual relationships in language processing.

**Concepts Demonstrated:**
- Natural language processing (NLP)
- Transformer-based deep learning
- Contextual relationships and attention
- Sequence-to-sequence translation
- Differences between classification and text generation

**Purpose:** Demonstrate why deep learning architectures are useful for language tasks that require contextual understanding and sequence generation.

**Important:** This is an educational simulation, not a trained or validated Transformer model. Its functionality illustrates translation concepts rather than actual neural network inference.

## Skills Demonstrated

- **AI/ML Fundamentals:** Understanding traditional machine learning and deep learning concepts.
- **Technical Research:** Reviewing and comparing academic studies and real-world applications.
- **Analytical Reasoning:** Evaluating model suitability, trade-offs, and limitations.
- **Model Workflow Understanding:** Illustrating classification and sequence-generation processes.
- **Technical Communication:** Translating research findings into accessible visual and explanatory materials.
- **Responsible AI:** Recognizing the importance of validation, interpretability, and human oversight.

## Project Value

This project demonstrates how technical research can be translated into practical considerations for business analytics and decision-making.

The churn prediction example illustrates how organizations might use structured data to identify retention risks, while the translation example demonstrates the potential of deep learning for contextual language processing.

Together, they reinforce a broader principle:

**The appropriate AI/ML solution depends on the analytical objective, available data, and practical constraints—not simply the sophistication of the algorithm.**

## Methodology and Limitations

The research paper is based on published academic and industry literature.

The classifier and translator examples are educational demonstrations intended to illustrate model workflows. They are not presented as production-ready solutions, independently validated predictive systems, or evidence of model performance.

No empirical performance claims are made for these illustrative examples.

### AI Assistance Disclosure

Generative AI was used to assist with research, writing revisions, infographic design, and development of two interactive educational simulations.

The simulations were created to communicate the conceptual workflows of customer churn classification and neural machine translation. They do not train machine learning models, perform validated neural network inference, or establish predictive performance.

The research paper provides the academic foundation, while the infographic and simulations adapt its central findings for a professional portfolio audience.
## References

- Gordini, N., & Veglio, V. (2017). Customers churn prediction and marketing retention strategies. *Industrial Marketing Management, 62*, 100–107.
- Grinsztajn, L., Oyallon, E., & Varoquaux, G. (2022). Why do tree-based models still outperform deep learning on typical tabular data? *Advances in Neural Information Processing Systems, 35*.
- NLLB Team. (2024). Scaling neural machine translation to 200 languages. *Nature, 630*, 841–846.
- Vaswani, A., et al. (2017). Attention is all you need. *Advances in Neural Information Processing Systems, 30*.

---

**Course:** AIML-500 — Machine Learning Fundamentals  
**Institution:** Indiana Wesleyan University  
**Author:** Yu-Hsuan Tseng

