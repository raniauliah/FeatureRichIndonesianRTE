# Feature Rich Indonesian RTE
This is Python implementation for the work that accepted on ACLing 2021 with paper entitled, "A Feature-Rich Classifier for Recognizing Textual Entailment in Indonesian".

Recognizing Textual Entailment (RTE) is a task in Natural Language Processing that can be used to determine the entailment of a sentence from another sentence. In this work we extract 35 features from a pair of text (T) and hypothesis (H) in Indonesian. We aim to solve the RTE task in Indonesian using a feature-rich classifier. 

## Dataset
The dataset used in this paper is **WRETE Dataset** that can be accessed [here](https://github.com/indobenchmark/indonlu/tree/master/dataset/wrete_entailment-ui). 
We only used the train data for the training process and test data to test the model. As explained on the paper, the class distribution in shown below

## Resource
**Word2vec Model**: [idwiki_word2vec_300.model](https://drive.google.com/file/d/1uuRSTsKpB3lbKYDYLIuCpLukBzKiipOS/view?usp=sharing)

**Pretrained Model POS Tagger**: [CRF Tagger](https://drive.google.com/open?id=12yJ82GzjnqzrjX14Ob_p9qnPKtcSmqAx) -- [read more](https://yudiwbs.wordpress.com/2018/02/20/pos-tagger-bahasa-indonesia-dengan-pytho/)

## Environment
This work was implemented on [Google Colaboratory](https://colab.research.google.com/)

### Sastrawi
`pip install sastrawi` -- [read more](https://pypi.org/project/Sastrawi/)

### NLTK
`pip install nltk` -- [read more](https://www.nltk.org/install.html)

### sklearn-crfsuite
`pip install sklearn_crfsuite` -- [read_more](https://pypi.org/project/sklearn-crfsuite/)

## Results
After performing an ablation study, the best performance in this work is obtained when using SVM with an F1-Score of 79.65%

## How To Run
1. `IPython Notebook/preprocessing.py` is the code implemented to preprocess both the train and test data. 
2. `IPython Notebook/model_processing.py` is the code implemented to train the model using all extracted data in the preprocessing step. The testing scenario also implemented in this code.


For further information, please email me at: [rani.auila@ui.ac.id](mailto:rani.auila@ui.ac.id) or [raniaulia72@gmail.com](mailto:raniaulia72@gmail.com)
