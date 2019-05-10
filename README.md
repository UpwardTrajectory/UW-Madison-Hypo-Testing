# University of Wisconsin - Madison: 
# Courses & Grades Analysis
----------------
### 2019.05.10

### Team David Kaspar & Hussein Sajid

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

Here is the final output from this notebook:

| Easiest Professors       | Ratio of A's | Other profs' Ratio |
|--------------------------|--------------|--------------------|
| 'Joseph Strand'          | 0.8          | 0.234              |
| 'Lindsay Hogan Garrison' | 0.7551       | 0.2331             |
| 'Leland Pan'             | 0.7345       | 0.2305             |
| 'Douglas Adams'          | 0.6923       | 0.2342             |
| 'Dominique Salas'        | 0.6667       | 0.2343             |
| ----------------------   | -----------  | ------------------ |
| **Hardest professors**     | **Ratio of A's** | **Other profs' Ratio** |
| 'Christopher Butler'     | 0.0408       | 0.2359             |
| 'Joelle Tybon'           | 0.04         | 0.2355             |
| 'Monica Styles'          | 0.04         | 0.2355             |
| 'Victoria Lantz'         | 0.0385       | 0.2355             |
| 'James Matenaer'         | 0.0312       | 0.2362             |


Joseph Strand is expected to give a ratio of A's between 31.7592 and 72.5886%. An instructor was not fair, and gave 80.00% A's, vs other instructors: 23.46%. This instructor was giving the most A's to their students in the respective course.

Christopher Butler is expected to give a ratio of A's between 20.7964 and 59.2036%.
Christopher Butler was not fair, and gave 4.0% A's, vs other instructors: 23.59%. This instructor was giving the lowest A's to their students in the respective course.


In a different notebook, we analyzed the overall average GPA from all classes that reported A-F style, completely omitting any (pass / fail) or other student achievement reporting methods. After transforming the possible grades: [A, AB, B, BC, C, D, F] onto the 4.0 GPA scale, we computed the weighted average based on class size for the entire dataset. We then randomly sampled 2000 records and computed a confidence interval for the population mean GPA utilizing bootstrapping for an empirical result.

[Bootstrapping Sample Test](uw_mad_grades_bootstrapping.ipynb)
