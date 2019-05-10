# Module 2 Final Project
----------------
### 2019.05.10

### Hypo-testing-UW-madison - Team David Kaspar & Hussein Sajid

[Final Jupyter Notebook](uw_mad_grades.ipynb)

[Slides](https://docs.google.com/presentation/d/1C4CV7enURSi7Ly9QkoGdXZ9F8CA36--hx4BYSOw9V2I/edit?usp=sharing)

**Project Goal**

The goal of this project is to test our ability to gather information from a real-world database and use our knowledge of statistical analysis and hypothesis testing to generate analytical insights that can be meaningful to the company/stakeholder.

**Statistical Analysis Requirements**

The goal of our project is to query the database to get the data needed to perform a statistical analysis. In this statistical analysis, we will need to perform a hypothesis test to answer at least one of the questions from the database you choose. 

For each hypothesis, be sure to specify both the null hypothesis and the alternative hypothesis for our question. We should also specify if this is one-tail or a two-tail test.

-----------------

## Introduction

The University of Wisconsin - Madison publishes reports for all courses (and sections of these courses), instructors, subjects, and grade reports for each section for every Fall and Spring semester since 2006.
There are more than 9,000 courses in this dataset. There are nearly 200,000 course sections with grades, with 3 million grades reported in total. 18,000 instructors are included in the dataset, all of whom are associated with various sections that may or may not have grades reported for them.

## Dataset: UW-Madison Wisconsin grades
Found [here (link to kaggle.com)](https://www.kaggle.com/Madgrades/uw-madison-courses)

We analyzed the overall average GPA from all classes that reported A-F style, completely omitting any (pass / fail) or other student achievement reporting methods. After transforming the possible grades: [A, AB, B, BC, C, D, F] onto the 4.0 GPA scale, we computed the weighted average based on class size for the entire dataset. We then randomly sampled 2000 records and computed a confidence interval for the population mean GPA utilizing bootstrapping for an empirical result.
