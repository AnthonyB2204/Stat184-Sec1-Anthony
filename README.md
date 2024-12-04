# Introduction
This repository contains an analysis of a Berkeley admissions dataset from 1973. The data examines admissions across different majors, broken down by gender, and whether the applicants were accepted or rejected. This project explores potential biases in admissions.

# Implementation
The analysis was implemented using:

Data Wrangling: The dataset was cleaned and prepared using R's ggplot2 and dplyr libraries.
Visualization: Visualizations were created to analyze trends, such as acceptance rates across genders and majors.
Quarto Markdown: The results and methodology are documented in a Quarto Markdown file (Vivian the Second of Atlanta.qmd) to produce an easy to follow analysis.

Here is an example of the code where I break down majors by gender:
```{r}
applications_gender_major <- data %>%
  select(Major, Gender) %>%
  group_by(Major, Gender) %>%
  summarize(
    Total = n()
  )
```
# Results
The analysis highlighted disparities in admissions rates based on gender and major. For example:

Majors with higher male applicants exhibited higher acceptance rates overall.
Visualizations, such as bar charts and pie charts, provided a clear view of these patterns.

Here is the graph generated from the previous code's analysis:
![image](https://github.com/user-attachments/assets/7cf89a3a-d95d-4d48-9353-c791df2148dd)

I concluded that the difference in admission rates is more closely related to the major that someone is applying to.
# Contact
For inquiries about this project, feel free to reach out via email: ajb848@psu.edu
