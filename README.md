# Topsis on Text Summarization Models
In this assignment we had to apply topsis to find the best pre-trained model for Text-Summarization

The dataset was taken from hugging face

The original dataset was having 12500 rows so I reduced the size of rows(you can use the whole train_df if you need better understanding but for the sake of simplicity I reduced the rows)

## I have taken 4 parameters for each text summarization model which are:
### 1.Semantic Coherence:
Impact: Semantic coherence measures how well the generated summary maintains the logical flow and coherence of the original dialogue. Higher semantic coherence indicates better flow and coherence.
### 2.Factual Accuracy:
Impact: Factual accuracy evaluates how accurately the generated summary represents the content of the original dialogue compared to the human-written summary. Higher factual accuracy indicates better representation of factual information.
### 3.Content Coverage:
Impact: Content coverage assesses the extent to which the generated summary covers important information from the dialogue. Higher content coverage indicates better coverage of relevant information.
### 4.Fluency:
Impact: Fluency measures the readability and coherence of the generated summary. Higher fluency indicates smoother and more natural-sounding summaries.

## The pretrined models that I have used are:
### 1.facebook/bart-large-cnn
### 2.t5-large
### 3.sshleifer/distilbart-cnn-12-6
### 4.google/pegasus-large
### 5.allenai/led-large-16384-arxiv

The results were stored in [evaluation_results.csv](https://github.com/gandhi25samar/Topsis_Assignment2-102103145/blob/main/evaluation_results.csv)

On this csv file Topsis was performed using my own package at Pypi which can be installed and used as:
#### Installation
```pip install Topsis-Samarjeet-102103145```
#### Usage
```Topsis evaluation_results.csv "1,1,1,1" "+,+,+,+" final_result.csv```
The result with topsis was stored in [final_result.csv](https://github.com/gandhi25samar/Topsis_Assignment2-102103145/blob/main/final_result.csv)

A graph was plotted of each model and its topsis score which is <img width="877" alt="Topsis_Graph" src="https://github.com/gandhi25samar/Topsis_Assignment2-102103145/assets/95834377/dbecddbe-2a40-40d4-9a5d-009a752ed696">
