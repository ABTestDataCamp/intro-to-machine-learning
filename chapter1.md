---
title       : "Machine Learning: Opening up the Black Box"
description : "A General Introduction to Machine Learning"
attachments :
  slides_link : https://s3.amazonaws.com/assets.datacamp.com/course/teach/slides_example.pdf


--- type:PlainMultipleChoiceExercise lang:r xp:50 skills:1 key:ef1b76935a
## The Buzzword

The term "Machine Learning" has been around for a while now, but to many it remains a mysterious black box. How does it really work? 

This course will teach you about the process of doing Machine Learning, from getting data to improving the accuracy of the models you will create.  

This course is for people that want to dive right in and get their hands dirty. By the end of the course, you should better understand what's inside the "black box".  

According to Wikipedia, Arthur Samuel in 1959 defined Machine Learning as the subfield of computer science that gives computers the ability to learn without being explicitly programmed.
This means that machines will be given the ability to make inferences and observation by learning from data. In other words, **machine learning is the science of teaching the machine to identify trends and patterns in data that cannot easily be detected by humans.**


### `CLASS ACTIVITY:`
From the above definition, which of the following is not a Machine Learning Task?

*** =instructions
- Self driving cars
- A program that prints the next 20 leap years
- A program that categorizes emails into spam and non-spam
- Predicting galaxies

*** =hint
Take a look at the options. Which task requires explicitly programming the computer?

*** =pre_exercise_code
```{r}
# None


```

*** =sct
```{r}
# SCT written with testwhat: https://github.com/datacamp/testwhat/wiki

msg_bad <- "That is not correct!"
msg_success <- "Exactly! Even I can calculate the next 50 leap years and I'm only human."
test_mc(correct = 2, feedback_msgs = c(msg_bad, msg_success, msg_bad, msg_bad))
```

--- type:PlainMultipleChoiceExercise lang:r xp:100 skills:1 key:c57adfc430

## A Model - The Secret Weapon

A human can learn the voices of 10 (or perhaps 100) co-workers and be able to identify them without looking. A machine, however, can learn the voices of over 10,000 people and be able to predict whose voice it is. How? Machine Learning!

Processes involved in Machine Learning include the following:

- Get data
- Preprocessing (Clean, Prepare, Manipulate Data & Exploratory Data Analysis)
- Train Model
- Test Model
- Post-Process (Visualize, Evaluate, Improve Model & Present)

The first two steps are typical for any analysis involving data.
Creating a model is a critical part of machine learning.

A model is an artifact or a formula created by the process of learning from previous data.
When you plug in historical data into a machine learning algorithm, you get a model.

In the above example, the machine uses a model that takes in an input (a person’s voice), does some processing and predicts the name of the person as the output. 

In chapter 3, you learn how to test, evaluate, and improve your model.


### `CLASS ACTIVITY:`

A good machine learning model depends on which of the following? 

*** =instructions
- Type of the data and software or statistical tool used for analysis
- Type of machine learning algorithm used and software or statistical tool used for analysis
- The quality of the dataset and type of machine learning algorithm used
*** =hint
Clean historical data + Good Machine Learning algorithm = Great Model!
*** =pre_exercise_code
```{r}

```

*** =sample_code
```{r}

```

*** =solution
```{r}

```

*** =sct
```{r}
# SCT written with testwhat: https://github.com/datacamp/testwhat/wiki

msg_bad <- "That is not correct!"
msg_success <- "Exactly!"
test_mc(correct = 3, feedback_msgs = c(msg_bad, msg_bad, msg_success))
```