---
title       : How Much Will I Earn?
description : This chapter introduces the decision tree algorithm. You will learn about random forest algorithm - a variant of the decision tree that improves it and performs better in general. Using random forest algorithm, you will create a model to predict what a person will earn based on their age, education and type of job.



--- type:MultipleChoiceExercise lang:r xp:100 skills:1 key:fbaf1d5d30
## Decision Tree Algorithm

Decision tree is a type of `supervised learning` algorithm and is mostly used in `classification` problems. This algorithm involves splitting the population or sample into two or more subpopulation based on most significant splitter in input variables.

Suppose we have a sample of `30 students` with two input variables `Gender` (Boy / Girl) and `Height` (5 to 6 ft). 15 out of these 30 play `Basketball` in leisure time. Students in red play basketball and those in blue do not. Let’s say we want to create a model to predict who will play basketball during leisure period? Basically, we want to separate students who play basketball in their leisure time based on highly significant input variable among all two variables (a.k.a. predictors)


Decision tree is useful here in that it will segregate the students based on all values of two variable. The variable which creates the best similar sets of students (i.e. sets which are dissimilar to each other). 



 ![](http://s3.amazonaws.com/assets.datacamp.com/production/course_4925/datasets/dtree.png)




In the figure above, you can see that variable Gender is able to identify best subpopulation sets compared to the variable height.



The `Random Forest` algorithm is a variant of decision tree algorithm. The algorithm involves constructing a multitude of decision trees at training time and outputting a result that is the `mode class` or `mean prediction` of the individual trees. This makes random forest `very accurate` and popular among data people.


### `CLASS ACTIVITY:`
Use `help(randomForest)` to find the documentation for randomForest package. 
Study the manual and answer the question below:

Which of the following argument is used to specify the number of trees to grow?

*** =instructions
- mtry
- nodesize
- forest
- ntree

*** =hint
- Type `help(randomForest)` in the R console to find the documentation for randomForest package.

*** =pre_exercise_code
```{r}
install.packages('randomForest')
library(randomForest)


```

*** =sct
```{r}
# SCT written with testwhat: https://github.com/datacamp/testwhat/wiki

msg_bad <- "That is not correct!"
msg_success <- "Exactly!"
test_mc(correct = 4, feedback_msgs = c(msg_bad, msg_bad, msg_bad, msg_success))

```
