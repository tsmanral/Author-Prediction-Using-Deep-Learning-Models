<h1 align="center"> Author Prediction Using Deep Learning </h1>

<p align="center">
<a href="https://tsmanral.github.io/" target="_blank"><img alt="Website" src="https://img.shields.io/badge/-Portfolio-informational"></a>
<a href="https://twitter.com/tribhuwan50" target="_blank"><img alt="Twitter" src="https://img.shields.io/twitter/follow/tribhuwan50.svg?style=social&label=Follow"></a>
<a href="https://www.linkedin.com/in/tribhuwan-singh-9411a175/" target="_blank"><img alt="LinkedIn" src="https://img.shields.io/badge/-Connect-blue?style=flat&logo=linkedin"></a>
<a href="https://github.com/tsmanral" target="_blank"><img alt="Github" src="https://img.shields.io/github/followers/tsmanral.svg?style=social"></a>
</p>

The project is aimed at the creation and analysis of multiple deep learning models for the task of author prediction, in order to carry out a quantitative comparison of the performance accuracies of these models and
ascertain the optimal model for this task.

The Corpus of English Novels (CEN), compiled by Hendrik De Smet, has been designed to allow tracking of short-term language change and comparing usage across individual authors. It consists entirely of novels, written by twenty-five novelists, both British (including Irish) and North American. In order to access this corpus of English Novels, we contacted Hendrik De Smet and thus obtained access to it. All novels are written between 1881 and 1922. All authors are born between 1848 and 1963 and represent roughly one generation of novelists. This corpus is used as the dataset for the machine learning models. The machine learning models are trained on the original text and the grammatical structure singly. Multiple neural network architectures namely, Feedforward Neural Networks, Convolutional Neural Networks and Recurrent Neural Networks (Long Short Term Memory) are implemented and analyzed.

The project applies deep learning and Natural Language Processing methodologies. We also make use of pre-trained networks such as Stanford’s POSTagger and GloVe, to make model training faster. POSTagger is used to convert the original text into its corresponding grammatical structure called Parts of Speech (POS). The GloVe network is used to get the pre-trained weights for the words, which are used in the embedding layer of the network, in order to make the machine learning model faster. To make the training faster, we deploy the models on the cloud. Also, we use the Natural Language Tool Kit (nltk) for pre-processing the data in order to clean it. The models are built using open-source deep learning frameworks namely, Tensorflow and
Keras.

In total, six different machine learning models are created: Feedforward Neural Network with original text, Feedforward Neural Network with grammatical structure, Convolutional Neural Network with original text, Convolutional Neural Network with grammatical structure, LSTM Recurrent Neural Network with original text, and LSTM Recurrent Neural Network with grammatical structure. The performance accuracies of the training, validation and test sets are compared for all six models.

The models trained on the grammatical structure outperform the models trained on the original text for every architecture. LSTM Recurrent Neural Networks outperform the other two networks when trained on original text. Moreover, all three models give almost equal performance in the case of training on grammatical structure.

### Dataset Details
We only used the subset of this corpus as the dataset for the machine learning models. The dataset we used in this project only consists of novels written by those authors who have written more than fifteen novels. These authors are summarized in the table below.

| Author              | Number of Novels | Year of Publication | Number of words |
|---------------------|------------------|---------------------|-----------------|
| Arthur Conan Doyle  | 18               | 1888-1913           | 1,566,987       |
| George Gissing      | 20               | 1884-1905           | 2,408,767       |
| Gilbert Parker      | 16               | 1893-1921           | 1,398,355       |
| Henry Rider Haggard | 25               | 1885-1910           | 2,556,621       |
| Humphrey Ward       | 19               | 1881-1916           | 2,252,823       |
| TOTAL               | 98               | 1881-1921           | 10,183,553      |

### Results

Metrics for models trained on original text:

| Model     | Training Accuracy | Training Loss | Validation Accuracy | Validation Loss | Testing Accuracy | Testing Loss |
|-----------|-------------------|---------------|---------------------|-----------------|------------------|--------------|
| FNN       | 86.175%           | 0.399         | 85.75%              | 0.413           | 83.878%          | 0.450        |
| CNN       | 89.3%             | 0.294         | 85.87%              | 0.396           | 86.38%           | 0.376        |
| RNN(LSTM) | 97.6%             | 0.11          | 90.69%              | 0.487           | 89.94%           | 0.475        |

Metrics for models trained on grammatical structure:

| Model     | Training Accuracy | Training Loss | Validation Accuracy | Validation Loss | Testing Accuracy | Testing Loss |
|-----------|-------------------|---------------|---------------------|-----------------|------------------|--------------|
| FNN       | 99.86%            | 0.004         | 99.6%               | 0.008           | 99.84%           | 0.006        |
| CNN       | 99.96%            | 0.002         | 99.87%              | 0.003           | 99.74%           | 0.006        |
| RNN(LSTM) | 99.91%            | 0.009         | 99.62%              | 0.038           | 99.39%           | 0.078        |

All accuracy and Loss graphs can be found in the **Accuracy_and_Loss_graphs** folder.

**Note:** This project was created as my final year project during my undergraduate degree at DIT University, Dehradun, India. I created this along with my teammate Yashvardhan Jain ([@J-Yash](https://github.com/J-Yash)).
