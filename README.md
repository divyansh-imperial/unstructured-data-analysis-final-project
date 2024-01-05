# Unstructured Data Analysis Final Project

This project is undertaken by Divyansh Saxena (CID - 01424151), MSc student at Imperial College London. As part of this project, I have implemented various data analytics and machine learning techniques on text data.

### Preface

The dataset used for this project consist of conversations by Updraft users with the customer support team. Updraft is fintech company based in UK with London HQ with 500,000+ users. We at Updraft provides a lending product (on iOS and Android) to users with existing loans of high interest rates. Our lending product has a much less interest rate that helps our users come out of the debt cycle fast and thus helping them make better financial decisions. The original dataset consisted of aroudn 16,000+ batched CSVs with a total size of 2.82 GB. This dataset was cleaned, pre-processed to have 277,741 rows and 6 columns with size of 145 MB or 33.5 MB of compressed CSV.

### Objective

Our analysis had four main objectives - 

- Find the main topics/ themes of conversations between Updraft users and the customer support team using topic modelling techniques.
    - Implement Latent Semantic Analysis from scratch using SVD and TF-IDF.
    - Dimension reduction of SVD output using PCA and tSNE for visualisation
    - Implement LSI model using gensim package 
- Perform exploratory analysis on the processed and filtered data to extract insights about the conversations to better understand the nature of the dataset.
    - Bar plots, Pie charts
    - Histograms
- Find pattern between topic and different days of week and topic and different hours of the day.
- Implement sentiment analysis using 3 different approaches to understand topics that are most frustrating for Updraft users.
    - VADER (Rule based lexical method)
    - BERT based Transformer model using Hugging Face (Default)
    - Advanced BERT based Transformer model using Hugging Face (bertweet-base-sentiment-analysis)

### Instructions to run code

1. Clone this repository and navigate to the root of this repository on terminal.
2. Open jupyter notebook from this path using `jupyter notebook` and open **UDA_FinalProject_Saxena_Code.ipynb**.
3. Run each code block sequentially.


> Note 1 - There is one code block in the beginning of the jupyter notebook that has this comment - ############## DO NOT RUN THIS CODE BLOCK ##############. As stated, no need to run this code as this code was a pre-processing step to combine, clean 16,000+ `.jsonl` files into a single dataset of 277741 x 6 dimension.

> Note 2 - Towards the end of the jupyter notebook there are codeblocks for implementing 2 transformer models on the whole corpus. They take around 3-4 hours to run in total. 

> Note 3 - Each figure shown in the PDF report has a corresponding comment in the jupyter notebook wherever it is generated.