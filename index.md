# TITLE: Dog Breeds Analysis
## Team Members: Kalynn Rhew, Avery Holder, and Colin Rogers
## Date: 12/10/2020

# Problem Statement and Motivation

The problem that our project aims to solve is matching people with their perfect dog breed based on characteristics they choose to input. We are all dog lovers and showed pictures of our dogs during our first meeting.

# Introduction and Description of Data
This problem is important because there are many dogs in shelters and sometimes it can be challenging to find the right dog for you. All of us have been through dog adoption processes and know how hard it can be to find the right dog. It is challenging since a lot of this information is all over the place and not consolidated in one single graph. Also, many people may have different qualities they look for in a dog so we will have to ensure the option to choose which qualities to rank.

Below is a bar graph ranking the 5 dogs with the highest mean score and their relative category scores.

![Top 5 Dogs](/images/top5.png)


We also created a function that would create an individual bar graph for each dog breed. Below is an example of one.

![An example of an individual dog's scores](/images/example_dog_graph.png)

# Literature Review/Related Work 
This study explores the personality traits of dogs and personality does and does not change from puppyhood to adulthood. The researchers found that aggressiveness and submissiveness were the most constant traits, but that response to training was the least consistent. https://www.ncbi.nlm.nih.gov/pmc/articles/PMC3553070/

Title: What Dog Breed is That? Description: Determining the breed of a dog using deep learning. This application has the goal of creating a classifier capable of determining a dog’s breed from a photo. https://towardsdatascience.com/dog-breed-identification-e3c6d6b4be84

Title: Best in show: The Ultimate Data Dog Description: This shows a visualization of a ranking of different dog breeds.

The Criteria were intelligence, costs, longevity, grooming, ailments, and appetite. https://www.informationisbeautiful.net/visualizations/best-in-show-whats-the-top-data-dog/

# Modeling Approach
The baseline model was originally a plot of the absolute/relative error using linear regression.
We also decided that in addition to the linear regression that we would impliment A K-NN model with ten neighbors. This was similar to the approach taken in problem set 3
  

We tried linear regression but that did not seem to communicate the relative error as well as we desired. Due to this we decided to impliment additional approaches. 
We noticed that there was more of a pattern in the relative error on the results provided by the K-NN approach. Below is the linear plot we tried to make of the error. 

![An example of linear regression on the data, which did not work.](/images/lin_reg.png)

Next, we decided to try using Classification with KNN, which we decided was a better modeling approach for this problem.

![An example of K-NN which seemed to work much better.](/images/knn.png)


# Project Trajectory, Results, and Interpretation 

At the start of our project, we were a little confused about how to approach this topic. It seems like Classification was the most fitting choice to 'classify' the dogs into breeds that different owners may like.

Throughout this project, we first cleaned the data using all of the tools we learned through class. This allowed us to better analyze relationships between variables and breeds.

# Conclusions and Future Work
In the future, it would have been smart if we did a prediction model that predicted what breed an owner would want, instead we chose a classification approach that also worked. 

To further this work, we could have created classified groups that dog breeds can be placed in. 

# Support Materials
Read about our setup for gathering and cleaning [here](https://github.com/AveryHolder/cpsc4300/blob/gh-pages/gather_and_clean.ipynb).

Read about our processing and conclusions [here](https://github.com/AveryHolder/cpsc4300/blob/gh-pages/process.ipynb).

# Declaration of academic integrity and responsibility

In your report, you should include a declaration of academic integrity as follows:

```
With my signature, I certify on my honor that:

The submitted work is my and my teammates' original work and not copied from the work of someone else.
Each use of existing work of others in the submitted is cited with proper reference.
Signature: Kalynn Rhew, Avery Holder, and Colin Rogers Date: 12/10/20
```

# Credit
The above project template is based on a template developed by Harvard IACS CS109 staff (see https://github.com/Harvard-IACS/2019-CS109A/tree/master/content/projects).
