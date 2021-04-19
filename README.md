![](https://img.shields.io/badge/PyTorch%20-%23EE4C2C.svg?&style=for-the-badge&logo=PyTorch&logoColor=white)
![](https://img.shields.io/badge/pandas%20-%23150458.svg?&style=for-the-badge&logo=pandas&logoColor=white)
![](https://img.shields.io/badge/numpy%20-%23013243.svg?&style=for-the-badge&logo=numpy&logoColor=white)
![](https://img.shields.io/badge/python%20-%2314354C.svg?&style=for-the-badge&logo=python&logoColor=white)
![](https://img.shields.io/badge/Jupyter%20-%23F37626.svg?&style=for-the-badge&logo=Jupyter&logoColor=white)
![](https://img.shields.io/badge/Twitter%20-%231DA1F2.svg?&style=for-the-badge&logo=Twitter&logoColor=white)


---
# Twitter Sentiment Analysis
Binary classification experiments for the Twitter dataset

###  Notebook viewer

‼️ Because of memory restrictions, GitHub and Browsers can't open  always big jupyter notebooks. 
For this reason I have every notebook linked with the ✔️ jupyter nbviewer ✔️ in the following table. 
If you have any problems opening the notebooks, follow the links.  


|Notebook | Link to jupyter nbviewer | Link to Colab |
|:-:|:-:| :-:| 
| __BiRNN_LSTM_GRU-BestModel.ipynb__  | [![nbviewer](https://raw.githubusercontent.com/jupyter/design/master/logos/Badges/nbviewer_badge.svg)](https://nbviewer.jupyter.org/github/Nikoletos-K/Twitter-Sentiment-Analysis/blob/main/BiRNN_LSTM_GRU-BestModel.ipynb) | [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://drive.google.com/file/d/1xXIoCKbuI-46RLNUy-ANK0mH7Vks5DPg/view?usp=sharing) |
| __BiRNN_LSTM_GRU-Experiments.ipynb__ | [![nbviewer](https://raw.githubusercontent.com/jupyter/design/master/logos/Badges/nbviewer_badge.svg)](https://nbviewer.jupyter.org/github/Nikoletos-K/Twitter-Sentiment-Analysis/blob/main/BiRNN_LSTM_GRU-Experiments.ipynb) |[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://drive.google.com/file/d/1QAi4BWk4YgmWbR-WhO7cQfoH7314CPVa/view?usp=sharing) |
| __FeedForwardNN_GloVe.ipynb__ |  [![nbviewer](https://raw.githubusercontent.com/jupyter/design/master/logos/Badges/nbviewer_badge.svg)](https://nbviewer.jupyter.org/github/Nikoletos-K/Twitter-Sentiment-Analysis/blob/main/FeedForwardNN_GloVe.ipynb) | [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://drive.google.com/file/d/106zQPt0H7PKVXwyJjZR1bXZrhEskhrkZ/view?usp=sharing) |
| __FeedForwardNN_TfiDf.ipynb__ | [![nbviewer](https://raw.githubusercontent.com/jupyter/design/master/logos/Badges/nbviewer_badge.svg)](https://nbviewer.jupyter.org/github/Nikoletos-K/Twitter-Sentiment-Analysis/blob/main/FeedForwardNN_TfiDf.ipynb) | [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://drive.google.com/file/d/1VEdLJaIr8xkMj6VYmyuSNfs7CzDJ_7kw/view?usp=sharing) |
| __LogisticRegression.ipynb__ | [![nbviewer](https://raw.githubusercontent.com/jupyter/design/master/logos/Badges/nbviewer_badge.svg)](https://nbviewer.jupyter.org/github/Nikoletos-K/Twitter-Sentiment-Analysis/blob/main/LogisticRegression.ipynb) | [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://drive.google.com/file/d/10EBO7COB6RVyJKFe70w80gk0nphv8yhr/view?usp=sharing) |



---
## Logistic regression
Developed a sentiment classifier using logistic regression for the Twitter sentiment classification dataset available in this [link](https://drive.google.com/file/d/1dTIWNpjlrnTQBIQtaGOh0jCRYZiAQO79/view?usp=sharing). I used the
toolkit Scikit-Learn again. 

### Vectorization: Tf-Idf
Tf-Idf vectorization of the tweets. No pretrained vectors

### Evaluation
Model metrics for evaluation: F1 score, Recall and Precision

Visualization: Confusion matrices

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

Visualization: ROC curves, Loss vs Epochs, Accuracy vs Epochs and Confusion matrix

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

Visualization: ROC curves, Loss vs Epochs, Accuracy vs Epochs and Confusion matrix

---

© Konstantinos Nikoletos | 2020 - 2021
