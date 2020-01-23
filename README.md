# Predicting-tags-using-spark-and-python
predicting Tags based on body text using spark and python

#### -- Project Status: [In-progress]

## Project Intro/Objective
Our goal is to create a predictive model which predicts post Tags based on Body and Title. To simplify the task and reduce the amount of code, we are going to concatenate Title and Body and use that as a single text column.

It might be easy to imagine how this model should work in the stackoverflow.com web site — the user types a question and the web size automatically gives tags suggestion.

Assume that we need as many correct tags as possible and that the user would remove the unnecessary tags. Because of this assumption we are choosing recall as a high priority target for our model.

To simplify our the first Apache Spark problem and reduce the amount of code, let’s simplify our problem. Instead of training a multi-label classifier, let’s train a simple binary classifier for a given tag. For instance, for the tag “Java” one classifier will be created which can predict a post that is about the Java language.

test