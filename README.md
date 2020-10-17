# Abstractive-Text-Summariser-With-NLP
*By Nethra Viswanathan, Brindha Mariappan, Hemapriya Kishorevenkatram*

Text Summarization recapitulate the content available in articles, research paper, news, paragraph or a piece of information. Automatic Text Summarization is made possible in Natural Language Processing (NLP) by employing two types of summarization techniques viz., 1) Extractive Summarization and 2) Abstractive Summarization. Extractive summarization generates summary by extracting the verbatim from the original passage whereas Abstractive summarization generates summary either by paraphrasing or by using new words instead of extracting the main points. A comprehensive news article and summary dataset has been chosen from Kaggle and the latter method of summarisation is employed in our coursework which calls for an abstractive modelling approach using sequence to sequence Long Short-Term Memory (LSTM) model. BLEU scoring technique has been used for evaluating the accuracy of the model owing to the extensive usage of the same for many of the models involving Natural Language Processing.

## DELIVERED FILES:
The model for text summarisation tool has been built and trained in Google Colab Pro which is a cloud
based solution for executing machine learning algorithms with availability of GPUs. Hence a Colab
notebook has been uploaded for execution from any system. The delivered zip file includes the
following:
1. Colab notebook “Abstractive_Text_Summariser.ipynb” to be executed in Google Colab since
only the missing libraries in Google Colab have been included in the *pip install* commands.
2. Two datasets – news_summary_more.csv which is the file used for training and validation and
news_summary_test.csv which has the test data to be demonstrated on the day of demo. (*Please send a request to nethra.viswanathan@gmail.com for dataset*)
3. Custom attention layer “attention.py” which is imported into the notebook
4. The weights of the trained model “s2s_lstm_weights_adam.h5” for testing the model. (*Not provided here*)
5. Figure “LossPlot.png” which is the plotted graph of training and validation loss stored as an
image for retrieval.
6. The text file “logswrite.txt” which has a record of the corpus and sentence wise BLEU score for a
subset of data in the validation dataset.
7. Environment file “environment.yml” for execution of code in local system if required.

## FILE PATH CONFIGURATION IN COLAB NOTEBOOK:
The current folder path needs to be assigned to the environment variable “PROJECT_PATH” as a onetime setup.

## IMPORTING DATASET IN COLAB PRO:
Dataset which is used for training the model needs to be placed in the drive and user needs to authorize
access for the google colab pro to work with files in drive for which the mounting command is also
provided in the notebook. Please enter the Google authorisation code to proceed with the execution
without issues.

## EXECUTION OF CODE in COLAB/LOCAL SYSTEM:
The code has been implemented in Google Colab Pro and hence it is recommended to execute the code
in Google Colab Pro. This is because the packages used in code are already installed in Colab and hence
exclusive installation statements are not provided as part of the notebook.
If the code needs to be executed in local system for any reason, please create the environment using
'environment.yml” file with the commands provided below before executing the notebook. The code has
been implemented in Python 3.7.

conda env create --file environment.yml
conda activate TextSummariser

