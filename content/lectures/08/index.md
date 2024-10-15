<h1 align="center">
<b>Lecture 08</b><br>
Paper 03 - Part 1
</h1>
<p align="center"><b>Date: </b>Oct 16, 2024</p>

**Today's paper:** Abramson, J., Adler, J., Dunger, J., Evans, R., Green, T., Pritzel, A., ... & Jumper, J. M. (2024). Accurate structure prediction of biomolecular interactions with AlphaFold 3. *Nature*, 1-3. DOI: [10.1038/s41586-024-07487-w](https://doi.org/10.1038/s41586-024-07487-w)

## Instructions

You will be working in your assigned group to present a key aspect of AlphaFold 3 methodology.
The focus should be on understanding how this part of the model works, rather than its history or applications.
Make sure to thoroughly explore the specific methodology behind your assigned topic.

### Research and Understanding

Begin by reading the relevant sections of the AlphaFold 3 paper that correspond to your group’s topic.
You are also encouraged to look up supporting references cited in the paper for deeper understanding.
As you research, think about why this methodology is important for AlphaFold 3.
Be prepared to explain not just how something works, but why it is critical for accurate protein structure prediction.

### Creating the Slides

Each group has a maximum of **12 minutes** for the presentation, plus an additional **3-5 minutes for discussion**.
Feel free to use the AlphaFold 3 paper and any other cited resources to enhance your understanding.
External sources are allowed, but make sure they are reputable and relevant.
If you use additional sources or diagrams, please include proper citations on your slides.
All members of your group should contribute to the presentation and participate in the delivery.
Decide in advance who will present which sections.

Your presentation should cover the following key components:

1.  **Introduction to Your Methodology**
    -   Briefly introduce the specific component of AlphaFold 3 your group is focusing on.
2.  **Step-by-Step Explanation**
    -   Use clear and detailed diagrams to walk through the core methodology.
    -   Break down complex concepts into smaller, digestible parts.
    -   Make sure to use relevant terminology and explain any new terms that appear in your presentation.
3.  **Key Technical Insights**
    -   Highlight the critical steps that make this method work effectively in AlphaFold 3.
    -   Provide examples (e.g., diagrams or charts) to show how the methodology improves prediction accuracy or efficiency.
4.  **Challenges or Limitations**
    -   Discuss any known challenges, limitations, or trade-offs of the method.
    -   Consider asking questions like: "What happens if this method doesn’t work as expected?" or "What are the limitations in certain cases?"
5.  **Summary and Discussion Questions**
    -   Conclude with a brief summary of your presentation.
    -   Prepare 1-2 critical thinking questions to ask the class, fostering discussion after your presentation.

#### Slide Presentation Guidelines

-   **Clarity and Simplicity**: Make sure your slides are not overcrowded. Focus on visuals (diagrams, flowcharts) to explain the concepts instead of large blocks of text.
-   **Explanation over Reading**: Do not just read off the slides. Instead, use the slides as a guide to explain the concepts in your own words.
-   **Engage the Audience**: Ensure your explanations are clear and structured in a way that the class can follow, especially since some topics will be technically challenging.
-   **Practice Timing**: Your group should aim for a **10-12 minute presentation** to allow time for class discussion afterward.

#### Leading the Discussion

-   **Prepare Questions**: After your presentation, you will lead a brief discussion by asking the class the **critical thinking questions** you prepared.
-   **Encourage Participation**: Make sure the discussion is interactive.
    Encourage classmates to share their thoughts and ideas about the methodology and any potential challenges they see.

## Rubric

Your presentation will be evaluated on the following:

-   **Understanding of the Topic**: How well does your group understand and explain the methodology behind AlphaFold 3?
-   **Clarity of Explanation**: Are the concepts presented clearly and logically? Are diagrams or visuals used effectively?
-   **Critical Engagement**: Does your group encourage the class to think critically about the method, its limitations, and its significance?
-   **Class Engagement**: Are the discussion questions thought-provoking and do they lead to meaningful class participation?

## Groups

Core Mechanisms in AlphaFold 3

### 1. Diffusion-Based Architecture in AF3

Begin by describing what a **diffusion model** is in general terms (this could be from research or other areas, like image denoising models). How do these models work by iterating and gradually improving an initial guess?
Look into why AlphaFold 3 would adopt this approach. Specifically, how does a diffusion-based model help with **protein structure prediction**, especially compared to AF2’s approach?

-   What does it mean that AF3 operates directly on **atomic coordinates**?
    How does this compare with AF2, which used more abstract representations (like torsion angles)?
-   What are the advantages of **predicting atomic coordinates directly** rather than going through intermediate steps?

Research the basic concept of how a **diffusion process** works.
How does AF3 take an initial guess of a protein’s structure and refine it through this iterative process?
-   Think about what challenges arise during the refinement of protein structures. For example:
    -   How might the initial structure be "noisy" or inaccurate?
    -   How does the diffusion model gradually refine the structure? What’s being corrected step by step?

-   Investigate how the diffusion process deals with **stereochemical errors**.
    What are these errors, and why are they problematic in protein structure prediction?
-   Explore the idea of **multiscale diffusion** in AF3.
    What might it mean to refine both **local** details (such as bond angles) and **global** features (such as the overall protein fold) at the same time?

Research and compare the traditional methods of structure prediction (such as in AF2) and the diffusion model introduced in AF3. How does the diffusion model simplify or improve upon earlier approaches?
Think critically about the trade-offs. Does this approach introduce any new challenges? For instance, are there any **computational costs** (time, resources, etc.) associated with using a diffusion-based model?

-   How might a **simpler prediction process** (working directly on atomic coordinates) lead to more accurate results?
    Are there any downsides to cutting out the intermediate steps used in AF2?
-   What are the potential **computational trade-offs** of using diffusion models? Do they require more processing power, time, or data?

### 2. Multiple Sequence Alignment (MSA) Processing in AF3

Begin by researching **what MSAs are** and why they’re important in protein structure prediction. How do they represent evolutionary relationships between protein sequences?
Compare how **AlphaFold 2 (AF2)** relied heavily on MSAs to extract evolutionary information. Then, explore the shift in **AlphaFold 3 (AF3)**, where there’s a **reduced emphasis on MSAs**. Why might this change have been introduced?

-   What is the **core function of an MSA** in guiding protein structure predictions? Why did AF2 rely so much on **MSA depth** (the number of sequences and evolutionary distance between them)?
-   Investigate the technical change in AF3—how does AF3 still maintain accuracy while relying less on deep MSAs? Look into how the **pairformer** module replaces the need for MSA depth in some cases.

Research the **reasoning behind AF3’s shift** from MSAs. Why was this shift necessary or beneficial? Think about the challenges that arose in AF2 when high-quality evolutionary data was not available.
Consider how AF3 compensates for this reduced dependence while still maintaining accurate predictions. What other mechanisms or methods (like the **pairformer**) does AF3 rely on to predict structure accurately without needing as much evolutionary information?

-   Look into the **drawbacks of relying on MSAs**: What happens when **evolutionary data is poor or absent** (e.g., for novel or rapidly evolving proteins)?
-   Explore the **pairformer module** in AF3. How does this module allow the model to maintain prediction accuracy without needing a deep evolutionary signal from MSAs?

Reflect on the importance of **evolutionary relationships** in structure prediction. How does evolutionary conservation help predict protein structure? What insights does MSA data provide, and why has it been a cornerstone of previous methods like AF2?
Then, think critically about **AF3’s innovation**: In cases where evolutionary information is weak or missing, how does AF3 continue to make accurate predictions? What alternatives or compensatory strategies does AF3 employ to make up for missing evolutionary data?

-   Investigate how AF3 processes **proteins with poor evolutionary information**. Are there cases where this new approach might fail or perform less effectively? How does the model balance accuracy without deep evolutionary data?
-   **Class Discussion Question**: "If evolutionary data is limited or absent, should we trust the structure predictions of AF3? How might this limitation affect its performance in predicting novel proteins?"

### 3. Pairformer Module vs. Evoformer

Begin by understanding the role of the **evoformer** module in AF2. This was a central component that processed multiple sequence alignments (MSAs) and pairwise features to generate structural predictions. Research how the evoformer used both sequence and pairwise data from MSAs to refine protein structure predictions.
Then, explore the **pairformer** module in AF3, which replaces the evoformer. How does this new module simplify the processing of **pairwise atomic relationships** while de-emphasizing MSA data?

-   What was the **purpose of the evoformer** in AF2? How did it integrate sequence and pairwise features?
-   What changes does the **pairformer** introduce in AF3? How does it handle **pairwise atomic representations** differently from the evoformer?
-   Look into how the **reduction in MSA dependence** has been balanced by the pairformer’s ability to work more directly with atomic interactions.

Research how the pairformer in AF3 **improves computational efficiency** compared to the evoformer. Focus on how AF3 simplifies the process of handling **complex atomic interactions** by focusing more directly on pairwise relationships between atoms, instead of relying on deep evolutionary sequence data.
Consider why this change was needed. What bottlenecks existed in AF2 due to its evoformer and reliance on MSA depth? How does the pairformer alleviate these issues?

-   Investigate why the pairformer can process pairwise representations **more efficiently** than the evoformer. What specific techniques does it use to handle the relationships between atoms in a protein structure?
-   Look into how AF3 handles **complex biomolecular interactions** (such as those in protein-ligand or protein-protein systems). How does the pairformer manage these interactions compared to the evoformer?

Reflect on the **impact of reducing MSA processing complexity** in AF3. The evoformer relied heavily on MSA features to predict structure in AF2, but the pairformer minimizes this dependency. Think about how this change improves **efficiency** but might also introduce challenges in cases where evolutionary data is limited.
Ask: Does reducing the complexity of MSA processing come at the cost of prediction accuracy? Or has AF3 managed to balance the need for evolutionary information in other ways, like more precise atomic pair interactions?

-   How does the pairformer’s **reduced reliance on MSAs** affect accuracy in cases where evolutionary information is rich versus when it’s sparse?
-   What are the potential **trade-offs** between speed and accuracy when simplifying MSA processing? Does the **pairformer compensate** for the reduced MSA complexity in other ways?

### 4. Template Search and Embedding in AF3

Start by understanding what **templates** are in the context of protein structure prediction. Templates are known structures (often from the Protein Data Bank, PDB) that serve as a reference when predicting the structure of an unknown protein.
In **AF2**, template use was important when sufficient **evolutionary data** (from MSAs) was unavailable or unreliable. AF2 searched for structural templates similar to the target protein and used them to guide predictions.
Investigate how **AF3** modifies this process. How does it search for and embed templates, and how is this process improved over AF2? Look into any changes in **template embedding and integration** that make AF3 more efficient or accurate.

-   Research how AF3 conducts **template searches**. What databases or resources does it pull from, and what specific features does it look for when identifying a useful template?
-   Explore how AF3 embeds these templates into its predictions. What changes in template integration have occurred between AF2 and AF3?

Dive into the **situations where AF3 relies on templates**. When evolutionary data is strong, AF3 can use MSAs to make accurate predictions. But when this data is weak or incomplete, AF3 needs templates to fill the gap.
Consider why **template-based predictions** are especially useful in some cases. For example, when predicting the structure of a protein with no strong homologs or evolutionary data, AF3 can use a **structural template** from a similar protein to guide the prediction process.

-   Investigate the **criteria** AF3 uses to decide whether to rely on a template. Are there specific thresholds (e.g., poor MSA data) that trigger template use?
-   Research how **template-based information** is incorporated into the model’s predictions. What specific role do these templates play in shaping the final structure?

Think about the **limitations of relying on templates**. While templates can help guide the structure of an unknown protein, they also come with risks. For instance, if the template isn’t a close match to the target protein, it could lead to incorrect predictions.
Ask: How does AF3 mitigate these issues? Research any strategies or techniques AF3 employs to avoid the pitfalls of **template over-reliance**.

-   Explore cases where templates **might introduce biases** into the prediction. For instance, if AF3 relies on a poor template, how might that affect the overall structure prediction?
-   Investigate how AF3 **balances template use** with other forms of data, like evolutionary information or direct atomic predictions, to ensure that predictions aren’t overly dependent on templates.
