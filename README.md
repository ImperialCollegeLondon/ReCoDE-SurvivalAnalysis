<!-- Your Project title, make it sound catchy! -->

# Cracking time's code: Survival analysis of large datasets

<!-- Provide a short description to your project -->

## Description

This is a special type of analysis that takes into consideration when the event occurred rather than if the event occurred. In other words, we are focused on acquiring the rate, which is the number of events per unit time. In this exemplar, I will introduce you to the concept of survival analysis (also known as a time-to-event analysis) using large datasets using R. Firstly, I will highlight the steps needed to effectively clean the data, including correct censoring of the participants.
Secondly, I will demonstrate two approaches: a univariable and a multivariable Cox Proportional regression model (which allows the incorporation of confounders). Thirdly, we will be able to estimate the hazard ratio of an event occurring between two groups and present our findings in a Kaplan-Meier curve(univariable analysis) or in a table/forest plot (multivariable).

This special type of analysis allows to calculate the risk of the event (disease, death, etc.) occurring at a given time (hazard ratio). A common timescale used in survival analysis is time-to-event, however in large cohort studies data may be left-truncated (participants entering the study at different time points), making the time-scale unsuitable. Instead, age should be considered as the timescale. This is most relevant when exploring age-dependent associations between exposures and outcomes. Therefore, it ensures accurate estimation of hazard risk and median survival times, preventing underestimation. In summary, survival analysis using large cohort data may be challenging and require throughout understanding of the data to ensure correct interpretability of the results.

<!-- What should the students going through your exemplar learn -->

## Learning Outcomes

- Understand the different types of censoring and how to curate your data 
- Conduct univariable and multivariable survival analysis using R
- Graphically present the findings of a survival analysis
- Interprete the results from a survival analysis

<!-- How long should they spend reading and practising using your Code.
Provide your best estimate -->

| Task       | Time    |
| ---------- | ------- |
| Pre-session material| 1.5 hours |
| Data curation| 2 hours |
| Analysis | 2 hours |
| Visualisation & Interpretation of results| 2 hours |
| Extension task | 1.5 hours |

## Requirements

<!--
If your exemplar requires students to have a background knowledge of something
especially this is the place to mention that.

List any resources you would recommend to get the students started.

If there is an existing exemplar in the ReCoDE repositories link to that.
-->

### Academic

<!-- List the system requirements and how to obtain them, that can be as simple
as adding a hyperlink to as detailed as writting step-by-step instructions.
How detailed the instructions should be will vary on a case-by-case basis.

Here are some examples:

- 50 GB of disk space to hold Dataset X
- Anaconda
- Python 3.11 or newer
- Access to the HPC
- PETSc v3.16
- gfortran compiler
- Paraview
-->

### System

<!-- Instructions on how the student should start going through the exemplar.

Structure this section as you see fit but try to be clear, concise and accurate
when writing your instructions.

For example:
Start by watching the introduction video,
then study Jupyter notebooks 1-3 in the `intro` folder
and attempt to complete exercise 1a and 1b.

Once done, start going through through the PDF in the `main` folder.
By the end of it you should be able to solve exercises 2 to 4.

A final exercise can be found in the `final` folder.

Solutions to the above can be found in `solutions`.
-->

## Getting Started

<!-- An overview of the files and folder in the exemplar.
Not all files and directories need to be listed, just the important
sections of your project, like the learning material, the code, the tests, etc.

A good starting point is using the command `tree` in a terminal(Unix),
copying its output and then removing the unimportant parts.

You can use ellipsis (...) to suggest that there are more files or folders
in a tree node.

-->

## Project Structure

```log
.
├── examples
│   ├── ex1
│   └── ex2
├── src
|   ├── file1.py
|   ├── file2.cpp
|   ├── ...
│   └── data
├── app
├── docs
├── main
└── test
```

<!-- Change this to your License. Make sure you have added the file on GitHub -->

## License

This project is licensed under the [BSD-3-Clause license](LICENSE.md)
