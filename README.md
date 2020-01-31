# Author Prediction Using Deep Learning Models
The project is aimed at the creation and analysis of multiple deep learning models for the task of author prediction, in order to carry out a quantitative comparison of the performance accuracies of these models and ascertain the optimal model for this task.

The Corpus of English Novels (CEN), compiled by Hendrik De Smet, has been designed to allow tracking of short-term language change and
comparing usage across individual authors. It consists entirely of novels, written by twenty-five novelists, both British (including Irish) and North American. All novels are written between 1881 and 1922. All authors are born between 1848 and 1963 and represent roughly one generation of novelists. This corpus is used as the dataset for the machine learning models. The machine learning models are trained on the original text and the grammatical structure singly. Multiple neural network architectures namely, Feedforward Neural Networks, Convolutional Neural Networks and Recurrent Neural Networks (Long Short Term Memory) are implemented and analyzed.

The project applies deep learning and Natural Language Processing methodologies. We also make use of pre-trained networks such as Stanford’s POSTagger and GloVe, to make model training faster. POSTagger is used to convert the original text into its corresponding grammatical structure called Parts of Speech (POS). The GloVe network is used to get the pre-trained weights for the words, which are used in the embedding layer of the network, in order to make the machine learning model faster. To make the training faster, we deploy the models on the cloud. Also, we use the Natural Language Tool Kit (nltk) for pre-processing the data in order to clean it. The models are
built using open-source deep learning frameworks namely, Tensorflow and Keras.

In total, six different machine learning models are created: Feedforward Neural Network with original text, Feedforward Neural Network
with grammatical structure, Convolutional Neural Network with original text, Convolutional Neural Network with grammatical structure, LSTM Recurrent Neural Network with original text, and LSTM Recurrent Neural Network with grammatical structure. The performance accuracies of the training, validation and test sets are compared for all six models


### RESULT
The models trained on the grammatical structure outperform the models trained on the original text for every architecture. LSTM Recurrent
Neural Networks outperform the other two networks when trained on original text. Moreover, all three models give almost equal performance in the case of training on grammatical structure.
