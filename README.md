# Twitter Sentiment Classifier
Binary classification experiments for the Twitter dataset

---
## Logistic regression
Developed a sentiment classifier using logistic regression for the Twitter sentiment classification dataset available in this [link](https://drive.google.com/file/d/1dTIWNpjlrnTQBIQtaGOh0jCRYZiAQO79/view?usp=sharing). I used the
toolkit Scikit-Learn again. 

### Vectorization: Tf-Idf
Tf-Idf vectorization of the tweets. No pretrained vectors

### Evaluation
Model metrics for evaluation: F1 score, Recall and Precision
Results visualization: Confusion matrices

---

## Feed-Forward Neural Net

Developed two sentiment classifier using feed-forward neural (__pyTorch__) networks for the Twitter sentiment
analysis dataset.

Experimented with:
- the number of hidden layers, and the number of their units
- the activation functions (only the ones presented in the lectures)
- the loss function
- the optimizer, etc

### Vectorization-1: Tf-Idf
Tf-Idf vectorization of the tweets. No pretrained vectors

### Vectorization-2: Pre-trained word embendding vectors - __GloVe__
Vectorization made with GloVe (Stanford pre-trained embenddings)

### Evaluation
Model metrics for evaluation: F1 score, Recall and Precision
Results visualization: ROC curves, Loss vs Epochs, Accuracy vs Epochs and Confusion matrix

---

## Bidirectional stacked RNN with LSTM/GRU cells

Experimented with:
- the number of stacked RNNs,
- the number of hidden layers, 
- type of cells,
- skip connections, 
- gradient clipping and 
- dropout probability

Used the __Adam optimizer__ and the binary cross-entropy loss function and transformed the predicted logits to probabilities using a __sigmoid__ function.

### Vectorization: GloVe
Pre-trained word embeddings (GloVe) as the initial embeddings to input on models.

### Evaluation
Model metrics for evaluation: F1 score, Recall and Precision
Results visualization: ROC curves, Loss vs Epochs, Accuracy vs Epochs and Confusion matrix

---

