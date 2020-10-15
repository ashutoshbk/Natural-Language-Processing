# Spam Classifier
   ![spam_mail](https://user-images.githubusercontent.com/49612207/96017202-56772000-0e67-11eb-8246-5ab0f046a720.jpg)

## Introduction

A collection of 425 SMS spam messages was manually extracted from the Grumbletext Web site.
The collection is composed of just one text file, where each line has the correct class followed by the raw message. We offer some examples below:

	ham What you doing?how are you?
	ham Ok lar... Joking wif u oni...
	ham dun say so early hor... U c already then say...
	ham MY NO. IN LUTON 0125698789 RING ME IF UR AROUND! H*
	ham Siva is in hostel aha:-.

So, I create two columns one independent and one dependent as per the above example.

## Setup
First, I imported all of the relevant libraries that I’ll be using as well as the data itself.

## Understanding Data
The collection is composed of just one text file. So, I create two columns "Label" and "Message".Where "Message" is an independent column and "Label" is dependent as per data.


## Missing Values
This is a very beginner-friendly dataset. I did not have to deal with any missing values, and there isn’t much flexibility to conduct some feature engineering given these variables. Next, I wanted to explore my data a little bit more.

## Preparing Data for Modelling
I prepare data in the following ways:
1. Remove all symbols and converted into small letters and merge into one paragraph by using lemmatization.
2. I use CountVectorizer to convert text into vectors.
	
## Split data
Next, I split the data into a training and test set so that I could cross-validate my models and determine their effectiveness.

## Modelling
For this project, I use Naive Bayes classifier to train a model.

![spamham](https://user-images.githubusercontent.com/49612207/96017233-60991e80-0e67-11eb-831a-2a639510633e.png)

## Result 
Naive Bayes Classifier gives 98.38 accuracies.

## Conclusion
By looking to this, we can see this high accurate model can predict whether message is Spam or Ham.
