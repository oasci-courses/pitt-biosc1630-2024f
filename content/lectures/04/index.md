<h1 align="center">
<b>Lecture 04</b><br>
Paper 01 - Discussion
</h1>
<p align="center"><b>Date: </b>Sep 18, 2024</p>

**Today's paper:** Champion, C., Gall, R., Ries, B., Rieder, S. R., Barros, E. P., & Riniker, S. (2023). Accelerating Alchemical Free Energy Prediction Using a Multistate Method: Application to Multiple Kinases. *Journal of Chemical Information and Modeling, 63*(22), 7133-7147. DOI: [10.1021/acs.jcim.3c01469](https://doi.org/10.1021/acs.jcim.3c01469)

## Introduction

**Duration:** 15 minutes

-   Welcome and session objectives (2 minutes)
-   Brief recap of the paper and its significance (5 minutes)
-   Explanation of the RE-EDS methodology and its context (5 minutes)
-   Overview of the session format and expectations (3 minutes)

## Small group discussions

Divide students into 4 groups, each focusing on a specific part of the **Results and Discussion**:

=== "**Group 1:** NF-κB Inducing Kinase (NIK)"

    **Guiding questions:**

    -   How might the structural differences among the NIK inhibitors (e.g., ring opening, fusion of rings) affect their binding mechanisms and the challenges in simulating them?
    -   What factors could contribute to the differences observed between GAFF and OpenFF force fields for NIK? How might these differences impact our understanding of protein-ligand interactions?
    -   Considering the role of Arg410 in NIK simulations, how might protein flexibility influence the accuracy of binding free energy calculations? What implications does this have for drug design?
    -   How do the results from RE-EDS compare to those from H-RE TI simulations for NIK? What might explain any differences observed?
    -   What are the potential advantages and limitations of using hybrid topology versus dual topology in the NIK simulations? How might this choice affect future free energy calculations?

    **Presentation (minimum) requirements:**

    -   Explain the structural differences among the NIK inhibitors
    -   Compare and contrast the results obtained with GAFF and OpenFF
    -   Discuss the role of Arg410 in the NIK simulations and its different conformations
    -   Present the comparison between RE-EDS and H-RE TI results
    -   Explain the differences between dual and hybrid topology simulations
    -   Present the key metrics (MUE, RMSE, Kendall τ, Spearman ρ) for NIK

    **Data:**

    -   Analyze Figure 6A and Table 1. Compare the performance of GAFF, OpenFF, and H-RE TI for NIK inhibitors. What trends do you notice in the calculated vs. experimental binding free energies?
    -   Examine Figure 6B. How does the choice of topology (dual vs. hybrid) affect the results for OpenFF? What might explain these differences?
    -   Study Figure 7 carefully. How do the different conformations of Arg410 relate to the simulation results? What does this suggest about protein flexibility in binding free energy calculations?
    -   Look at Figure S5 in the Supporting Information. How do the crystal structures of NIK inhibitors compare to the simulated conformations? What insights does this provide?
    -   Analyze the statistical metrics in Table 1 for NIK. What do these values tell you about the accuracy and reliability of the different methods and force fields?

=== "**Group 2:** p21-Activated Kinase 1 (PAK)"

    **Guiding questions:**

    -   How do the different types of heterocycle transformations in the PAK dataset reflect real-world drug optimization strategies?
    -   What molecular or structural features might explain the differences in accuracy between PAK and NIK results?
    -   How could the binding pose of PAK inhibitors and the hydrogen bond with Lys299 inform structure-based drug design efforts?
    -   What implications does the difference in dihedral angle sampling between GAFF and OpenFF have for force field development and selection in future studies?
    -   How might the findings from the PAK simulations, particularly regarding buried substituents, influence the design of next-generation kinase inhibitors?

    **Presentation (minimum) requirements:**

    -   Describe the PAK inhibitor modifications and their significance
    -   Compare the accuracy of PAK results to those of NIK
    -   Present the key metrics for PAK using both GAFF and OpenFF
    -   Explain the binding pose of PAK inhibitors and its impact on results
    -   Discuss the importance of the hydrogen bond with Lys299
    -   Analyze the differences in dihedral angle sampling between GAFF and OpenFF for PAK

    **Data:**

    -   Examine Figure 8A and Table 2. Compare the performance of GAFF and OpenFF for PAK inhibitors. Which force field seems to perform better, and why?
    -   Study Figure 8B carefully. How does the binding pose of ligand K.1 inform your understanding of the PAK inhibitor interactions?
    -   Analyze Figures 8C, 8D, and 8E together. What do these figures tell you about the differences in dihedral angle sampling and hydrogen bonding between GAFF and OpenFF?
    -   Look at the correlation metrics (Kendall τ and Spearman ρ) in Table 2. What do these values suggest about the ranking ability of each force field for PAK inhibitors?
    -   Compare the MUE and RMSE values for PAK with those of other kinases in the study. What does this comparison tell you about the relative difficulty of modeling PAK inhibitors?

=== "**Group 3:** Checkpoint Kinase 1 (CHK1)"

    **Guiding questions:**

    -   Why might studying different subsets of CHK1 inhibitors be important, and what can we learn from comparing their results?
    -   How do the results from this study compare to previous methods like FEP+ and QligFEP for the smaller CHK1 subset? What might account for any differences or similarities?
    -   What factors could contribute to the higher accuracy of CHK1 results compared to other kinases? How might this inform future computational studies?
    -   How could the performance differences between GAFF and OpenFF for CHK1 guide force field selection in future drug discovery projects?
    -   Based on the CHK1 results, what recommendations would you make for improving the accuracy of binding free energy calculations in kinase systems with solvent-exposed substituents?

    **Presentation (minimum) requirements:**

    -   Describe the two CHK1 subsets and their key characteristics
    -   Compare the results of the smaller subset to previous studies (e.g., FEP+, QligFEP)
    -   Present the key metrics for both CHK1 subsets
    -   Explain any differences in performance between GAFF and OpenFF
    -   Discuss factors that might contribute to the high accuracy of CHK1 results

    **Data:**

    -   Analyze Figure 9A and the corresponding data in Table 3 for the smaller CHK1 subset. How do the results compare across GAFF, OpenFF, and the previous GROMOS force field?
    -   Examine Figure 9B and the related data in Table 3 for the larger CHK1 subset. What differences do you notice between the two subsets, and what might explain these differences?
    -   Study Figure S8 in the Supporting Information. How do the RE-EDS results for CHK1 compare to other methods like FEP+ and QligFEP?
    -   Look at Figure S9 in the Supporting Information. What does the sampling distribution tell you about the efficiency of the RE-EDS method for CHK1 inhibitors?
    -   Compare the statistical metrics for CHK1 in Table 3 with those of other kinases in the study. What conclusions can you draw about the relative ease or difficulty of modeling CHK1 inhibitors?

=== "**Group 4:** Proviral Insertion in Murine Lymphoma Kinase 1 (PIM)"

    **Guiding questions:**

    -   How do the structural modifications in the PIM dataset, including bulky substituents, reflect current trends in kinase inhibitor design?
    -   What molecular or structural features might explain the differences in accuracy between PIM and CHK1 results?
    -   How could the challenges encountered with ligand M.4 (e.g., rearrangement of Arg122) inform future improvements in simulation protocols or force field parameterization?
    -   What are the potential implications of the performance differences between GAFF and OpenFF for PIM in the context of kinase drug discovery?
    -   How might the impact of bulky substituents on sampling and results influence the design and optimization of PIM inhibitors in the future?

    **Presentation (minimum) requirements:**

    -   Describe the structural modifications in the PIM inhibitor set
    -   Present the key metrics for PIM and compare them to CHK1
    -   Explain the challenges encountered, particularly with ligand M.4
    -   Compare the performance of GAFF and OpenFF for PIM
    -   Discuss the impact of bulky substituents on sampling and results

    **Data:**

    -   Analyze Figure 10A and Table 4. Compare the performance of GAFF and OpenFF for PIM inhibitors. What trends do you notice, and how do they differ from other kinases in the study?
    -   Examine Figure 10B carefully. How does the binding pose of ligands M.1 and M.4 inform your understanding of the challenges in modeling PIM inhibitors, especially those with bulky substituents?
    -   Study Figures S11 and S12 in the Supporting Information. What do these figures reveal about the differences in dihedral angle sampling between GAFF and OpenFF for ligand M.4?
    -   Look at Figure S10 in the Supporting Information. How does the sampling distribution for PIM compare to that of CHK1 (Figure S9)? What might explain any differences?
    -   Analyze the statistical metrics in Table 4 for PIM. How do these values compare to the null model, and what does this tell you about the performance of RE-EDS for PIM inhibitors?

---

For each group, consider

-   What were the main findings in this section?
-   How do these results compare to previous studies?
-   What limitations or challenges were identified?
-   What are the implications of these findings?
-   How does this section contribute to the overall narrative of the paper?

## Group Presentations

Each group presents their section (5 minutes each) and other groups ask questions after each presentation.

## Break

**Duration:** 10 minutes

## Critical Analysis Activity

This worksheet covers various aspects of the paper, encouraging students to engage deeply with the content, critically evaluate the methods and results, and consider the broader implications of the research.
It also promotes scientific thinking by asking students to propose future directions and reflect on their learning.
Students discuss in pairs (10 minutes), then share with the class (10 minutes)

### Part 1: General Understanding

1.  Briefly summarize the main objective of this study in your own words.
2.  Explain the key differences between RE-EDS and traditional pairwise free energy methods.
3.  List the four kinases studied and describe one unique feature of each kinase's inhibitor set.

### Part 2: Data Analysis

For your assigned kinase group (NIK, PAK, CHK1, or PIM), answer the following:

4.  Describe the main trends you observe in the calculated vs. experimental binding free energies.
5.  Compare the performance of GAFF and OpenFF force fields for your kinase. Which performed better and why?
6. Identify a specific challenge in modeling your kinase's inhibitors and explain its potential impact on the results.
7. Analyze the sampling distribution for your kinase. What does it tell you about the efficiency of the RE-EDS method?

### Part 3: Critical Evaluation

8. Identify 2 strengths of this study.
9. Identify 2 weaknesses or limitations of this study.
10. What additional experiments or analyses would you suggest to address the limitations or expand on the findings?
11. How might these findings impact the field of computational drug design, particularly for kinase inhibitors?
12. What ethical considerations might arise from this research and its potential applications?

### Part 4: Comparative Analysis

13. Compare the performance of RE-EDS across the four kinases. Which kinase showed the best results and why do you think this is the case?
14. Examine Figure 11 and related data. How does the computational efficiency of RE-EDS compare to traditional methods? What implications does this have for drug discovery?

### Part 5: Future Directions

15. Based on the study's findings, propose a specific research question or hypothesis for future investigation in this field.
16. Describe a potential application of the RE-EDS method outside of kinase inhibitor design. How might it be useful in other areas of drug discovery or computational chemistry?

### Part 6: Reflection

17. What aspect of this study did you find most interesting or surprising? Why?
18. How has this paper changed or reinforced your understanding of computational methods in drug design?
19. If you could ask the authors one question about their work, what would it be?

### Part 7: Communication

20. Create a brief (3-5 bullet points) summary of the key findings and significance of this study that could be understood by a non-expert audience.

## Break

**Duration:** 10 minutes

## Reflection

### Group Discussion

In small groups of 3-4, discuss the following:
1. What are the three most important takeaways from this study?
2. How does this research advance our understanding of computational drug design?
3. What challenges or limitations of the RE-EDS method did you identify?
4. How might this method impact the drug discovery pipeline in pharmaceutical companies?

### Summarize Key Points

As a class, create a list of the top 5 key points from the group discussions.

### Individual Reflection

Write a brief reflection addressing the following:

1. What is the most significant concept you learned from this paper? Explain why you find it important.
2. How has this study changed your understanding of:
    -   Computational methods in drug design?
    -   The challenges in predicting protein-ligand interactions?
1. Identify one aspect of the RE-EDS method that you'd like to understand better. Formulate this as a specific question.
2. Imagine you're explaining this research to a friend who isn't in science. Write 2-3 sentences summarizing why this work matters.
3. If you were to continue this research, what would be your next step or question to investigate?

### Closing Thought

Consider and jot down one way this research might influence your future studies or career interests.
