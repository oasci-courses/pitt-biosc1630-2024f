<h1 align="center">
<b>Lecture 06</b><br>
Paper 02 - Methods & Discussion
</h1>
<p align="center"><b>Date: </b>Oct 2, 2024</p>

!!! danger "DRAFT"

    This page is a work in progress and is subject to change at any moment.

**Today's paper:** Zhu, W., Zhang, Y., Zhao, D., Xu, J., & Wang, L. (2022). HiGNN: A hierarchical informative graph neural network for molecular property prediction equipped with feature-wise attention. *Journal of Chemical Information and Modeling, 63*(1), 43-55. DOI: [10.1021/acs.jcim.2c01099](https://doi.org/10.1021/acs.jcim.2c01099)

## Learning objectives

What you should be able to do after today's lecture:

1.  Compare and contrast different molecular representations.
2.  Describe basic concepts of neural networks and deep learning as applied to molecular property prediction.
3.  Explain the fundamental principles of Graph Neural Networks (GNNs) and their application.
4.  Describe the concepts of message passing and aggregation in GNNs.
5.  Discuss the role of attention mechanisms in neural networks for molecular property prediction.
6.  Describe the concepts of chemical fragments, pharmacophores, and molecular scaffolds.
7.  Describe the main components of HiGNN's architecture.

## Activity

For this journal club, you will be split into five groups, each responsible for presenting a portion of the paper *“HiGNN: A Hierarchical Informative Graph Neural Network for Molecular Property Prediction Equipped with Feature-Wise Attention”* by Zhu et al.
Each group will prepare a set of lecture slides during class and present for **10 minutes**, followed by a short Q&A.

Your task is to explain your assigned section clearly, ensuring your classmates understand the key points, and to engage the class in a discussion on the relevance and impact of the research.

1.  **Preparation Time:** You will have time in class to prepare your slides. Each group should create approximately **5-7 slides** for their presentation.
2.  **Presentation Time:** Each group will present for **10 minutes**, with an additional **5 minutes for questions** from the audience.
3.  **Content:** Summarize the key points of your assigned section. You are encouraged to include visuals (e.g., figures, tables) from the paper to aid understanding.
4.  **Discussion Questions:** At the end of your presentation, ask **2-3 questions** to engage the class in discussion about your section.
5.  **Teamwork:** Split the work evenly among group members. Each member should have a speaking role during the presentation.
6.  **Focus:** Highlight the core concepts, avoid getting too caught up in overly technical details unless they are essential to your section.

---

### Group 1: Introduction and Background

**Assigned Sections:**

- Introduction (pp. 43-45 in the paper)
- Abstract

**Your Goals:**

- Explain the challenge of predicting molecular properties in drug discovery.
- Discuss the importance of graph neural networks (GNNs) in addressing these challenges.
- Introduce the concept of HiGNN and how it improves upon previous methods.
- Highlight the significance of this research for the broader field of drug discovery.

**Suggested Slide Breakdown:**

1. Introduction to molecular property prediction.
2. Challenges and current methods in the field.
3. Introduction to GNNs and their applications.
4. The purpose and objectives of HiGNN.
5. A brief overview of the paper’s research questions and goals.

**Discussion Questions:**

- Why are current graph-based deep learning methods insufficient for molecular property prediction?
- How might HiGNN improve the drug discovery process in practical terms?

---

### Group 2: HiGNN Framework Architecture

**Assigned Sections:**

- Methods: HiGNN Architecture (pp. 45-47, covering molecular graph and BRICS fragmentation)

**Your Goals:**

- Provide a detailed explanation of the HiGNN architecture.
- Focus on the hierarchical design of HiGNN and how it processes both molecular graphs and BRICS fragments.
- Explain the role of the **feature-wise attention** mechanism in recalibrating atomic features.
- Highlight how these architectural innovations lead to improved molecular property predictions.

**Suggested Slide Breakdown:**

1. Overview of HiGNN architecture.
2. Explanation of molecular graph processing.
3. Introduction to BRICS fragmentation and its integration.
4. Description of the feature-wise attention mechanism.
5. How these components interact to improve predictions.

**Discussion Questions:**

- How does the hierarchical design of HiGNN differ from traditional GNNs in molecular property prediction?
- Why is the feature-wise attention mechanism a crucial innovation in this model?

---

### Group 3: Experimental Setup and Data Sets

**Assigned Sections:**

- Methods: Benchmark Data Sets and Hyperparameters (pp. 48-49)

**Your Goals:**

- Explain the benchmark data sets used in the study and why they are relevant for drug discovery.
- Discuss the importance of using multiple data sets for evaluating model performance.
- Provide an overview of the training process, including the hyperparameter optimization.
- Mention the significance of splitting the data into training, validation, and test sets.

**Suggested Slide Breakdown:**

1. Introduction to the data sets used in the study.
2. Relevance of each data set for molecular property prediction (mention a few key data sets like ESOL, FreeSolv, BACE, etc.).
3. Overview of the training process.
4. Hyperparameter optimization and its role in the study.
5. Significance of data splitting (random vs. scaffold splitting).

**Discussion Questions:**

- Why is it important to evaluate the model on a variety of data sets?
- How does scaffold splitting improve the generalizability of the model compared to random splitting?

---

### Group 4: Results and Performance Analysis

**Assigned Sections:**

- Results and Discussion (pp. 49-50)

**Your Goals:**

- Summarize the model’s performance on different data sets.
- Compare HiGNN’s performance with other models such as GCN, GAT, and Chemprop.
- Highlight key findings, especially in tasks related to drug discovery, such as predicting ADMET properties.
- Discuss why HiGNN outperformed other models in most cases and what that implies for future research.

**Suggested Slide Breakdown:**

1. Overview of performance results on key data sets.
2. Comparison of HiGNN with other models (focus on top-performing models).
3. Specific success stories (e.g., BACE, BBBP data sets).
4. Discussion of HiGNN’s strength in predicting ADMET properties.
5. What do these results mean for future applications?

**Discussion Questions:**

- In which areas does HiGNN significantly outperform other models, and why?
- What might be some limitations of HiGNN based on its performance across different tasks?

---

### Group 5: Interpretability and Case Studies

**Assigned Sections:**

- Interpretation of HiGNN: Case Studies on BACE and BBBP (pp. 50-52)

**Your Goals:**

- Explain the **molecular-fragment similarity mechanism** and its role in making HiGNN interpretable.
- Use the **BACE** and **BBBP** case studies to demonstrate how HiGNN identifies key molecular fragments.
- Discuss how this interpretability can aid chemists in drug design.
- Highlight the practical implications of the findings from the case studies.

**Suggested Slide Breakdown:**

1. Overview of HiGNN’s interpretability mechanism (molecular-fragment similarity).
2. Case study 1: BACE (show how HiGNN identifies key fragments).
3. Case study 2: BBBP (explain how permeability predictions work).
4. Importance of model interpretability in drug discovery.
5. Potential future applications of this interpretability.

**Discussion Questions:**

- How does the molecular-fragment similarity mechanism improve the interpretability of HiGNN’s predictions?
- Why is interpretability important in drug discovery models?
