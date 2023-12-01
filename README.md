# NER_with_transformers

This repository contains code for training and evaluating Named Entity Recognition (NER) models on the [MultiNERD dataset for English](https://colab.research.google.com/corgiredirector?site=https%3A%2F%2Fhuggingface.co%2Fdatasets%2FBabelscape%2Fmultinerd). Two systems, A and B, are developed and compared. System A is fine-tuned on the English subset of the original dataset, while System B is further fine-tuned on a filtered dataset containing only five entity types (PERSON, ORGANIZATION, LOCATION, DISEASES, ANIMAL) and the O tag. The base model used for these systems is DistilBERT uncased.

## Environmental Setup

Create a virtual environment and install the required dependencies

```
pip install -r requirements.txt
```

OR
Use Google colaboratory and uncomment the installations cell.

## Code

Run multinerd_ner_systemA to build System A and evaluate it on the test dataset. Repeat for System B with multinerd_ner_systemB.

## Primary Findings

See findings.txt for a short commentary on the systems' performance
