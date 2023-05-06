# Prescription Parser using CRF

This project implements a doctor prescription parser using the CRF (Conditional Random Fields) algorithm. The parser takes a prescription (sentence) as input and labels the words in that sentence with pre-defined labels using sequence prediction.

## Problem Statement

Given a prescription in the form of a sentence split into tokens, the task is to label each word in the sentence with one of the pre-defined labels. The output labels are as follows:

- Method
- Qty
- Form
- Frequency
- Period
- PeriodUnit
- FOR
- Duration
- DurationUnit

## Input Data

The input data consists of a list of prescription sentences in the form of tokens, and the corresponding output labels.

## Implementation

The implementation is done in Python using the following libraries:

- nltk
- sklearn_crfsuite
- sklearn
- spacy

The following steps are performed to build the prescription parser:

1. The training data is created by splitting the sentence into tokens, computing POS (Part of Speech) tags, and creating triples of the form (word, pos_tag, label).

2. Features are extracted from the training data using the CRF algorithm.

3. The data is split into training and testing sets.

4. The CRF model is created and trained using the training set.

5. The model is saved to a file for future use.

6. The saved model is loaded and used to predict labels for the test data.

7. The accuracy of the model is evaluated using various metrics such as F1 score, confusion matrix, and classification report.





## Conclusion

The CRF-based prescription parser implemented in this project is capable of  predicting the labels for prescription sentences with an accuracy of 86.7%. The model can be trained on a larger dataset to improve its accuracy further.
