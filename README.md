# Project Name
> Healthcare Disease Treatment Labeling Assignment


## Table of Contents
* [Problem Statement](#problem-statement)
* [Assumptions](#assumptions)
* [Technologies Used](#technologies-used)
* [Final Model](#final-model)
* [Conclusions](#conclusions)
* [Acknowledgements](#acknowledgements)
* [Contacts](#contacts)


## Problem Statement
- Now, let’s consider a hypothetical example of a health tech company called ‘BeHealthy’. Suppose ‘BeHealthy’ aims to connect the medical communities with millions of patients across the country.

‘BeHealthy’ has a web platform that allows doctors to list their services and manage patient interactions and provides services for patients such as booking interactions with doctors and ordering medicines online. Here, doctors can easily organise appointments, track past medical records and provide e-prescriptions.

So, companies like ‘BeHealthy’ are providing medical services, prescriptions and online consultations and generating huge data day by day.

Let’s take a look at the following snippet of medical data that may be generated when a doctor is writing notes to his/her patient or as a review of a therapy that he or she has done.

“The patient was a 62-year-old man with squamous cell lung cancer, which was first successfully treated by a combination of radiation therapy and chemotherapy.”

As you can see in this text, a person with a non-medical background cannot understand the various medical terms. We have taken a simple sentence from a medical data set to understand the problem and where you can understand the terms ‘cancer’ and ‘chemotherapy’.

Suppose you have been given such a data set in which a lot of text is written related to the medical domain. As you can see in the dataset, there are a lot of diseases that can be mentioned in the entire dataset and their related treatments are also mentioned implicitly in the text, which you saw in the aforementioned example that the disease mentioned is cancer and its treatment can be identified as chemotherapy using the sentence.

But, note that it is not explicitly mentioned in the dataset about the diseases and their treatment, but somehow, you can build an algorithm to map the diseases and their respective treatment.

Suppose you have been asked to determine the disease name and its probable treatment from the dataset and list it out in the form of a table or a dictionary like this.

After discussing the problem given above, you need to build a custom NER to get the list of diseases and their treatment from the dataset.

## Assumptions
- NA


## Technologies Used
- Language - Python
- library - Numpy
- library - Pandas
- library - sklearn_crfsuite
- library - spacy
- Library - nlkt
- Library - sklearn


## Final Model
- We have defined the following features for CRF model building:

f1 = input word is in lower case;

f2 = last 3 characers of word;

f3 = last 2 characers of word;

f4 = True; if the word is in uppercase, False otherwise;

f5 = True; if word is a number; otherwise, False

f6 = True; if the word starts with a capital letter; otherwise, False

f7 = True; if the word is Noun or Proper Noun; otherwise, False

f8 = POS TAG of the word

f9 = frequency of the word in the full corpus

f10 = previous word is in lower case;

f11 = True; if the previous word is in uppercase, False otherwise;

f12 = True; if previous word is a number; otherwise, False

f13 = True; if the word starts with a capital letter; otherwise, False

f14 = True; if the word is Noun or Proper Noun; otherwise, False

f15 = POS TAG of the word

## Conclusions

- we got a F1 score of 91%


## Acknowledgements
- This project is part of a case study from Upgrad for labeling disease and treatment for an input file


## Contacts
- Created by [@debimahapatra]
