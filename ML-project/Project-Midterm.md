# Project Report Title
**Authors** : Jakob Ramirez, Alex Cummins, William Langley, Saron Abebe

**Abstract** : It is a standalone section. It is written to give the reader a summary of your work. Be sure to specific, yet brief. Even though the abstract comes first in your paper, it is sometimes easier to write the abstract last. (150-300 words)

## Introduction

Your project report is the formal description of your project. The format is similar to the presentation but we want you to fully elaborate on what you did. You could provide some background knowledge about the data you are analyzing, clearly and concisely present your research question, describe the dataset that can help answer your question. (0.5-1 page) 

**Note:** you can transform it to Jupyter Notebook and add sections below as markdown cells. 

## Problem Statement 
  
The goal of this project is to design a model to predict which schools are high poverty stricken based on publicly available data in the United States. The benchmark we are using is the one that was provided to us in the class, we are using it because it was convenient and it has interesting implications about the state of the education system in the United States. The data comes from the Department of Education's database on public education in the United States, the Common Core of Data.
  
We hope to be able to use Machine Learning to create a model that can accurately predict the likelyhood of a poverty stricken school given data that does not direclty correlate to poverty probability. We think reduced price lunch is a key feature inorder to predict Title I schools.

### Related Work

Those affected by the data found, of which schools are high poverty stricken, include but are not limited to residents who are in need of financial support, potential residents seeking specific relocation preferences, and scholarship targets searching where to begin. This data will could provide clairty in patterns of which areas are next or begin solution to decrease the effects. 


## Data Management 

In this section you should address the questions of interest and interpret the results in terms of the questions of interest you proposed. (1-5 pages, including relevant tables and figures, please adjust your figures to appropriate sizes).

- Describe how did you evaluate your solution
- What evaluation metrics did you use?
- Describe a baseline system
- How much did your system outperform the baseline?
- Were there other systems evaluated on the same dataset? How did your system do in comparison to theirs?
- Show graphs/tables with results
- Error analysis
- Suggestions for future improvements

Description of the dataset (dimensions, names of variables with their description)

### Data Gathering

Using the table generator to collect the data of public schools, filtered to only get schools in the states of Texas, Arkansas, Oklahoma, Louisiana and, New Mexico. The columns chosen were school name, county name, title I eligible, total students (all grades exlcluding adult education) and, reduced-price lunch eligible students. The time range of data chosen is 2008-2018(most recent available) because, the great recession began in 2008 which drastically changed the economy.

### Data Pre-processing, Cleaning, Labeling, and Maintenance 

Stored the downloaded data into different dataframes according to year. Data can be accessed from different yearly dataframes using a dictionary(keys=year, value=dfs). Dropped na values for each yearly dataframe resulting in different amounts of data per dataframe. Data can also be grouped by state as well.

### Exploratory Data Analysis 

* Describe the methods you explored (usually algorithms, or data wrangling approaches). 
* Justify your methods in terms of the problem statement. 
* What did you consider but *not* use? In particular, be sure to include every method you tried, even if it didn't "work". 
**NOTE:** Move from .md to .ipynb format when you plan to show EDA (either project proposal or midterm checkpoint)

## Machine Learning Approaches

In this section, you could describe the methods you used in your analysis. For example, if you are doing classifications, you could introduce the methods like logistic regression, discriminant analysis, support vector machines. You don't have to write formulas if you don't want to do so. It is fine to describe the methods in words. This section basically is a description of the methodologies that you have used for analyzing your data. (up to 2pages)
Describe the choice of Machine Learning Tool.  Refer ro related work, if applicable.  

* Evaluate a primary model and in addition a "baseline" model. 
  * The baseline is typically the simplest model that's applicable to that data problem
    * Naive Bayes for classification
	* K-means on raw feature data for clustering.
* Evaluate state-of-art model 
  * Research gitHuib, paperswithcode, Kaggle and similar. 
  * If not applicable, talk to the instructor.  
  
**Hint** Goal is to have some sort of baseline evaluation by Nov 11th checkpoint to establish a scale by which to measure your project's performance. Compare the performance of your baseline model and primary model and explain the differences.

** This is where all the methods you have tried go, including state-of-art if any **

### Describe the ML methods that you used and the reasons for their choice. 
What is the family of machine learnign algorithms you are using and why? 
* Supervised or Unsupervised?
* Regression or classification?

### Justify ML algorithms in terms of the problem itself and the methods you want to use. 
* How did you employ them? 
* What features worked well and what didn't?
* Provide documentation for integration  

### Tools and Infrastructure Tried and Not Used

Describe any tools and infrastruicture that you tried and ended up not using.
What was the problem? 
Describe infrastructure used. 

## Experiments

Give a detailed summary of the results of your work.

 * Setup - Here is where you specify the exact performance measures you used.  
   * Describe the data used in experiment for presenting dataset: Datasheets for Dataset template 
   * Describe your accuracy or quality measure, and your performance (runtime or throughput) measure. 
   
 * Please use visualizations whenever possible. Include links to interactive visualizations if you built them. 
 
 * You can also submit a separated notebook as an appendix to your report if that makes the visualization/interaction task easier. 
   * It would be reasonable to submit your report as a notebook, but please make sure it runs on one of the two standard environments, and that you include any required files. 

## Conclusion
In this section give a high-level summary of your results. If the reader only reads one section of the report, this one should be it, and it should be self-contained.  You can refer back to the Experiments Section for elaborations. This section should be less than a page. In particular emphasize any results that were surprising.


## References
List the references that cited in your project.

## Appendix## 

Explain the contributions of each member to the project. Include all supporting materials, e.g., additional figures/tables, Python code technical derivations.
