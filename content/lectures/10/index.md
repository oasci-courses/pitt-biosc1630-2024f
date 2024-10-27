<h1 align="center">
<b>Lecture 10</b><br>
Paper 04 - Reading
</h1>
<p align="center"><b>Date: </b>Oct 30, 2024</p>

**Today's paper:** Buttenschoen, M., Morris, G. M., & Deane, C. M. (2024). PoseBusters: AI-based docking methods fail to generate physically valid poses or generalise to novel sequences. *Chemical Science, 15*(9), 3130-3139. DOI: [10.1039/D3SC04185A](https://doi.org/10.1039/D3SC04185A)

This class period is dedicated to forming groups, reading and analyzing the PoseBusters paper, and beginning work on your group presentations.
Each group will focus on one specific aspect of the study and prepare a structured presentation to be delivered in class next week, following the peer editing of your analysis drafts.

1.  **Forming Groups**
    -   You will divide into five groups, each assigned a unique section of the PoseBusters study to analyze in depth.
    -   Make sure each group has a balanced mix of strengths, with students who can contribute to various aspects of the presentation, including research, visual design, and oral delivery.
2.  **Reading and Analyzing the Paper**
    -   Once groups are formed, read through the PoseBusters paper together, focusing on the section assigned to your group.
    -   Discuss and take notes on the methodology, results, and key insights related to your group’s specific topic (e.g., docking protocols, validation criteria, performance comparison, energy minimization, or binding site considerations).
    -   As you read, pay attention to any supplemental materials (SI) that might provide additional data or visuals to support your presentation.
3.  **Planning and Drafting Your Presentation**
    -   Begin planning your presentation outline using the provided instructions for each group. Decide on key points, visuals, and examples to include for clarity.
    -   Assign roles within the group, so each member knows which parts of the presentation they’ll focus on, from researching details to designing slides or delivering sections.
    -   Remember that each presentation should be about **10-12 minutes long**, with clear visuals and explanations, engaging the audience in a discussion of your section’s insights.
4.  **Initial Slide Development and Content Organization**
    -   Start creating slides with a logical flow, using visuals to make complex points clear. Refer to charts, diagrams, or data in the SI as needed to enhance your explanations.
    -   Keep slides concise and visual-based, avoiding text-heavy slides. Instead, focus on using bullet points, flowcharts, and diagrams to illustrate major points.
5.  **Questions and Feedback**
    -   Use this time to ask questions and clarify any part of the paper or your group’s topic. I am here to help with any content, interpretation, or structure questions.
    -   Review the presentation instructions to ensure your group’s approach aligns with expectations and covers all key points.

## Groups

### **Group 1:** Docking Protocols and Setup Across Methods

Your goal is to introduce the docking protocols used in the PoseBusters study for each method.
This will set up a foundational understanding of how each docking method was configured and prepared for accurate comparisons.
Emphasize the importance of standardized setups in docking studies and why a consistent initial setup is essential for obtaining meaningful results, especially when comparing different methodologies.

1.  **Brief Overview of Docking Methods**
    -   *Instructions*: Begin with a concise summary of each docking method: DiffDock, DeepDock, EquiBind, TankBind, Uni-Mol, AutoDock Vina, and CCDC Gold.
    -   *Guidelines*:
        -   Provide a brief description of each method’s approach to docking (e.g., traditional scoring for AutoDock Vina and Gold vs. deep learning in DiffDock).
        -   Emphasize unique aspects of each method to clarify why certain setups might differ across methods.
2.  **Detailed Protocol and Setup**
    -   *Instructions*: Focus on the ligand and protein preparation steps used for each docking method.
    -   *Guidelines*:
        -   Describe ligand preparation, such as using RDKit’s ETKDGv3 conformer generation for ligand conformations.
        -   Detail the protein preparation, including hydrogen addition and binding site specifications (e.g., radius or distance thresholds) tailored for each method.
        -   Explain any deviations between methods and why these differences are necessary based on each algorithm’s requirements.
3.  **Importance of Consistency in Setup for Comparative Analysis**
    -   *Instructions*: Emphasize why the PoseBusters study applied a standardized protocol for each method, regardless of whether it was classical or DL-based.
    -   *Guidelines*:
        -   Explain that standardization allows for fairer comparisons, reducing bias introduced by varying preparation steps.
        -   Discuss the challenges in standardizing these protocols across fundamentally different methodologies (e.g., deep learning models vs. classical scoring-based models).

Wrap up your presentation by explaining that even with a consistent setup, assessing docking outcomes requires rigorous validation criteria to determine how well each method performs.

### **Group 2:** PoseBusters Validation Criteria

Your goal is to explain the three core categories of validation criteria used by PoseBusters to evaluate docking predictions. These criteria are essential for ensuring the chemical and physical reliability of docking outputs across different methods.
Focus on how these criteria—**chemical validity**, **intramolecular validity**, and **intermolecular validity**—collectively ensure predictions are meaningful and suitable for scientific analysis, ultimately contributing to the concept of **PB-validity**.

1.  **Overview of the Three Validation Criteria Categories**
    -   *Instructions*: Introduce the three main categories used in PoseBusters to evaluate docking outcomes.
    -   *Guidelines*:
        -   Begin with a general introduction to validation in docking studies and why rigorous criteria are essential for comparing methods.
        -   Briefly outline the three categories—chemical, intramolecular, and intermolecular validity—and note that each ensures predictions are accurate and feasible within the constraints of molecular biology and chemistry.
    -   *Slide Tips*: Create a clear, labeled diagram or flowchart that displays each validation category, perhaps with visual icons (e.g., chemical bonds for chemical validity, molecular structure for intramolecular validity).
2.  **Detailed Breakdown of Each Category**
    -   *Instructions*: Dive deeper into each category, explaining what each type of validity checks and why it’s necessary.
    -   *Guidelines*:
        -   **Chemical Validity**: Cover checks like RDKit sanitization, molecular formula preservation, and stereochemistry (e.g., chirality and double bond configurations).
        -   **Intramolecular Validity**: Discuss bond length and angle assessments, focusing on how these checks help prevent unrealistic molecular geometries.
        -   **Intermolecular Validity**: Explain checks for steric clashes, including protein-ligand minimum distances and volume overlaps with other molecules like cofactors.
        -   For each validity category, briefly mention the consequences if predictions fail these checks (e.g., chemically invalid ligands cannot function in biological systems).
    -   *Slide Tips*: Use individual slides or sections for each category, accompanied by brief explanations and relevant visuals (e.g., stereochemistry diagrams for chemical validity, bond angles for intramolecular validity).
3.  **The Concept of PB-Validity**
    -   *Instructions*: Introduce **PB-validity** (PoseBusters validity) as a cumulative measure of docking reliability.
    -   *Guidelines*:
        -   Explain how PB-validity represents an all-encompassing metric that indicates a pose passes all checks within the three categories, showing it is chemically, intramolecularly, and intermolecularly sound.
        -   Emphasize the advantage of PB-validity in offering a holistic measure of docking outcome reliability, aiding in the comparison of docking methods.
    -   *Slide Tips*: Create a visual representation or checklist showing how each criterion contributes to PB-validity, perhaps using a flowchart that ends in a “PB-validity” box for simplicity.
4.  **Importance of These Validation Steps**
    -   *Instructions*: Conclude by stressing the importance of these criteria in validating docking methods and ensuring that results are meaningful, particularly when comparing classical and DL-based docking approaches.
    -   *Guidelines*:
        -   Briefly mention how these criteria help address unique challenges posed by deep learning models versus traditional docking approaches.
        -   Reinforce that without these checks, docking predictions could result in unreliable poses that fail to reflect realistic protein-ligand interactions.
    -   *Slide Tips*: Summarize this point on a final slide to reinforce that validation is a critical bridge from protocol to performance, setting up Group 3.

Conclude by emphasizing that validation alone doesn’t reveal which methods perform best; performance outcomes must still be compared to understand the strengths and weaknesses of each approach.

### **Group 3:** Performance Comparison Between Classical and DL-Based Docking Methods

Your group’s goal is to compare the docking performance of classical methods (like AutoDock Vina and CCDC Gold) with deep learning (DL)-based methods (such as DiffDock, DeepDock, and EquiBind) using PoseBusters’ RMSD and PB-validity criteria.
Highlight the differences in accuracy and reliability between these two types of methods, focusing on how each performs under the validation checks established in PoseBusters.

1.  **Introduction to Performance Metrics (RMSD and PB-Validity)**
    -   *Instructions*: Start by briefly introducing RMSD (Root Mean Square Deviation) and PB-validity as the main metrics used to assess docking performance in PoseBusters.
    -   *Guidelines*:
        -   Explain **RMSD** as a measure of the positional accuracy of the predicted ligand pose compared to the experimental (or known) pose, with lower values indicating greater accuracy.
        -   Introduce **PB-validity** as a comprehensive measure that indicates a ligand pose meets all physical, chemical, and geometric validity checks.
    -   *Slide Tips*: Create a clear introductory slide with concise definitions or icons for RMSD and PB-validity. If helpful, add a small diagram showing the concept of RMSD to aid understanding.
2.  **Comparative Analysis of RMSD and PB-Validity Across Methods**
    -   *Instructions*: Present a comparative analysis of RMSD and PB-validity scores across classical and DL-based methods.
    -   *Guidelines*:
        -   Highlight how classical methods (AutoDock Vina and CCDC Gold) and DL-based methods (e.g., DiffDock, EquiBind) performed according to RMSD and PB-validity.
        -   Describe trends: for example, classical methods might have lower RMSD and higher PB-validity, while DL-based methods may have challenges in maintaining validity checks.
    -   *Slide Tips*: Use a comparison table, bar chart, or side-by-side visual (such as a waterfall plot from the SI) to display RMSD averages and PB-validity percentages for each method, emphasizing key differences.
3.  **Trends in Valid Pose Counts and Accuracy Differences**
    -   *Instructions*: Summarize broader trends in the number of valid poses and accuracy differences between classical and DL-based docking methods.
    -   *Guidelines*:
        -   Describe how classical methods generally produced more valid poses, meeting validation checks for geometry and physical feasibility, while DL-based methods struggled in some areas.
        -   Mention any specific DL methods that performed well or poorly on particular aspects, like bond angle accuracy or stereochemistry.
    -   *Slide Tips*: Consider a waterfall plot from the SI that shows valid and invalid pose counts, or create a line graph to show trends in valid pose counts across methods. Label peaks and dips to indicate which methods succeeded or failed in meeting PB-validity.
4.  **Strengths and Weaknesses of DL-Based vs. Classical Docking Approaches**
    -   *Instructions*: Conclude your performance comparison by discussing the strengths and limitations of DL-based and classical methods as observed in PoseBusters.
    -   *Guidelines*:
        -   **Classical Methods**: Highlight their robustness in producing PB-valid poses but note they may require more computational resources and time compared to DL-based methods.
        -   **DL-Based Methods**: Explain that while DL methods like DiffDock and EquiBind are fast and scalable, they often fall short in chemical and stereochemical accuracy, particularly without extensive validation or adjustments.
        -   Use specific examples from PoseBusters results to illustrate each point.
    -   *Slide Tips*: Create a summary table or chart contrasting DL-based and classical methods’ strengths and weaknesses. Include specific examples from the data to make this comparison more tangible.

Wrap up by noting that while the results highlight performance trends, **energy minimization** can further impact docking predictions by refining pose accuracy and addressing validity issues.

### **Group 4:** Effects of Energy Minimization on Docked Poses

Your objective is to analyze how post-docking energy minimization affects docking validity and prediction accuracy. This includes both the positive impacts (refining docked poses) and potential drawbacks (introducing inaccuracies).
By examining specific examples from the PoseBusters study, you’ll show that energy minimization is a double-edged sword, capable of both improving and compromising docking results.

1.  **Introduction to Energy Minimization in Docking**
    -   *Instructions*: Begin with a brief explanation of what energy minimization is and why it’s used in docking studies.
    -   *Guidelines*:
        -   Define **energy minimization** as a process that adjusts molecular geometries to reach a stable, low-energy conformation, typically using force fields like **AMBER** or **Sage**.
        -   Explain that energy minimization is intended to refine predicted ligand poses by resolving unrealistic geometries, bond lengths, and angles, thus increasing docking accuracy.
    -   *Slide Tips*: Use a simple diagram showing a ligand pose before and after energy minimization, highlighting changes in geometry or energy levels to introduce this concept.
2.  **Role of Force Fields (AMBER, Sage) in Refining Docked Poses**
    -   *Instructions*: Provide an overview of how force fields like AMBER and Sage contribute to energy minimization.
    -   *Guidelines*:
        -   Explain that these force fields model physical interactions (e.g., bond stretching, angle bending) to produce a realistic conformation by reducing strain.
        -   Mention any particular challenges associated with using force fields in energy minimization, such as computational expense or dependence on accurate parameterization.
        -   Discuss why these force fields are specifically used for biological molecules to achieve physically realistic docking poses.
    -   *Slide Tips*: Consider using a labeled diagram showing the types of molecular interactions (e.g., bond lengths, angles) that force fields optimize.
3.  **Examples of Energy Minimization Effects: Refinement vs. Distortion**
    -   *Instructions*: Present examples from the PoseBusters study showing both positive and negative impacts of energy minimization on docking results.
    -   *Guidelines*:
        -   Show examples where energy minimization successfully corrected geometric errors in DL-based poses, such as unrealistic bond angles or steric clashes.
        -   Highlight cases where energy minimization “destroyed” previously valid poses, introducing distortions that moved them away from realistic conformations.
        -   Emphasize that while energy minimization can correct certain errors, it’s not a guaranteed solution and can sometimes compromise docking accuracy.
    -   *Slide Tips*: Use before-and-after visuals from the PoseBusters study, such as specific ligand conformations pre- and post-minimization, to illustrate changes.
4.  **Visual Data Analysis: Mixed Results of Energy Minimization**
    -   *Instructions*: Use visual data to illustrate the mixed outcomes of energy minimization on docking validity.
    -   *Guidelines*:
        -   Present data from the PoseBusters SI, such as percentage of poses passing validation checks after minimization, to show the variability in results.
        -   Use waterfall or bar plots to highlight trends (e.g., increased validation for some methods, decreased for others), underscoring the inconsistency of energy minimization’s effects.
    -   *Slide Tips*: Include charts or waterfall plots from the SI showing performance metrics before and after energy minimization, emphasizing changes in PB-validity.
5.  **Complexity of Energy Minimization in Docking**
    -   *Instructions*: Conclude by discussing why energy minimization is a complex and nuanced process that can both help and hinder docking outcomes.
    -   *Guidelines*:
        -   Mention how energy minimization may cause oversimplification of molecular interactions, sometimes ignoring critical details needed for accurate docking.
        -   Discuss the challenge of balancing energy minimization’s corrective power with its potential to introduce artifacts or over-corrections, particularly in deep learning-based docking.
        -   Reinforce that while energy minimization can improve docking validity, it’s not always appropriate or effective across all docking methods.
    -   *Slide Tips*: Create a summary slide with bullet points listing both the benefits and drawbacks of energy minimization, giving the audience a balanced view.

Conclude by mentioning that energy minimization’s effectiveness can vary further in cases involving cofactors or complex binding sites, which present additional challenges to docking accuracy.

### **Group 5:** Influence of Cofactors and Binding Site Definitions on Docking Accuracy

Your group’s objective is to examine the effects of cofactors and binding site definitions on docking accuracy and validity within the PoseBusters framework.
You will highlight how proximity to cofactors and binding site size can impact docking results across methods, influencing the overall reliability of predictions.

1.  **Introduction to Cofactors in Docking**
    -   *Instructions*: Start with a brief overview of what cofactors are in the context of docking and why they matter.
    -   *Guidelines*:
        -   Define **cofactors** as non-protein, non-ligand molecules (e.g., metal ions, iron-sulfur clusters) found within or near the binding site, which often play critical roles in protein function and ligand binding.
        -   Explain why including cofactors in docking calculations can impact accuracy, as they contribute additional binding interactions and spatial constraints.
    -   *Slide Tips*: Use a labeled diagram showing a protein-ligand complex with cofactors in proximity to illustrate the concept visually.
2.  **Impact of Cofactors on Prediction Accuracy**
    -   *Instructions*: Discuss how cofactors affected docking prediction accuracy across methods in the PoseBusters study.
    -   *Guidelines*:
        -   Highlight findings showing that certain methods (e.g., DL-based methods like TankBind) may struggle more with predictions in the presence of cofactors.
        -   Summarize performance differences when cofactors are within a close proximity (e.g., 4.0 Å), noting any specific challenges or improvements in PB-validity when cofactors are included.
        -   Explain that methods handling cofactors more effectively often yield more PB-valid poses, as these poses respect the physical constraints introduced by the cofactor.
    -   *Slide Tips*: Use a comparison chart or bar graph from the SI showing PB-validity rates for predictions with and without cofactors, visually emphasizing the differences.
3.  **Binding Site Definitions and Their Effect on Accuracy**
    -   *Instructions*: Describe the impact of varying binding site definitions, focusing on the different settings used in Uni-Mol and CCDC Gold.
    -   *Guidelines*:
        -   Explain how the **binding site radius** (e.g., 6 Å vs. 8 Å) impacts the search area for ligand binding, influencing docking predictions by limiting or expanding the modeled environment.
        -   Compare Uni-Mol and CCDC Gold’s binding site definitions and how each approach affected PB-validity, with larger search areas (e.g., 8 Å) typically encompassing more potential binding interactions.
        -   Emphasize that adjusting the binding site definition alters both computational efficiency and accuracy, as it dictates the spatial constraints for docking calculations.
    -   *Slide Tips*: Use visuals from the SI, like diagrams showing different radii around binding sites, to illustrate how binding site definitions influence the scope of predictions.
4.  **Visual Data: Comparative Performance Under Different Binding Site Settings**
    -   *Instructions*: Present data from the SI to show how different binding site settings and cofactor inclusion impacted method performance.
    -   *Guidelines*:
        -   Include visuals such as bar graphs or waterfall plots showing PB-validity percentages or RMSD comparisons for different binding site radii.
        -   Highlight any clear trends, such as improved PB-validity at certain binding site definitions or reduced accuracy when binding sites are too large or too small.
        -   Discuss how cofactors influenced these results and whether specific methods performed better with optimized binding site configurations.
    -   *Slide Tips*: Use side-by-side charts for easy comparison, showing how PB-validity shifts with varying binding site radii or presence/absence of cofactors.
5.  **Key Takeaways and Summary**
    -   *Instructions*: Conclude with a summary of the main points on how cofactor proximity and binding site definitions impact docking accuracy and validity.
    -   *Guidelines*:
        -   Reinforce that the proximity of cofactors and careful selection of binding site radii are both crucial for accurate and reliable docking results.
        -   Connect back to previous validation and performance results, emphasizing that these factors can either improve or limit docking validity, depending on the setup.
    -   *Slide Tips*: Create a concise summary slide with bullet points listing the main takeaways on cofactors and binding site effects, linking these factors to overall docking reliability.

Wrap up by noting that carefully optimized binding site definitions and cofactor handling are essential for reliable docking predictions.
Highlight that both cofactors and binding site parameters are fine-tuning options that directly affect PB-validity and should be customized based on the docking method and protein-ligand system.
