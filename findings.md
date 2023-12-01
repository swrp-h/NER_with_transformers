For the purpose of this task, we do not consider accuracy given the typical imbalance in NER datasets, instead focusing on f-1 score, precision and recall. Both systems A and B demonstrate favourable results when evaluated on the test data, with both f-1 scores over 0.9 after the second epoch. The performance of system B is higher at an f-1 score of 0.95 (vs. 0.93 for system B), which can be attributed to the reduced set of its entity types (11 vs 31). This trend is mirrored by their corresponding precision (0.94 vs. 0.92) and recall (0.95 vs. 0.93) scores. 

The base model chosen for the task was a DistilBERT, a smaller, faster version of BERT with 40% less parameters (1), which can imply that finetuning an original BERT may result in a better performance. Continued experimentation can help test this. The model was also finetuned with default hyperparameters recommended by Hugging Face (2), and further optimization of these hyperparameters can result in even better, state-of-the-art results.

(1) https://huggingface.co/docs/transformers/model_doc/distilbert
(2) https://huggingface.co/docs/transformers/main/tasks/token_classification
