# deep_dive_covid19

This is a group project for CS525:Information Retrieval and Social Web. 02/03/2020-05/12/2020

The main purpose of this tool is to serve the research community members, whether it be scholars, grad school students, or science enthusiasts. Since the outbreak of the coronavirus pandemic, researchers around the world have been trying to get a basic understanding of this situation, how it originated, what’s the biological explanation behind this, and most importantly, how to prevent the potential further damage to human kind. There are multiple areas surrounding this issue, from sociology, chemistry to biology, and different scholars has their own unique understanding of this situation, therefore the amount of information and papers related to this disease might be overwhelming to some people, hence our tool would help filter the unwanted materials and render the most relevant ones to those who needed it based on their own preferences.

## Base Structure
Django

## Data source:
* [CORD-19-research-challenge](https://www.kaggle.com/allen-institute-for-ai/CORD-19-research-challenge)
* We used the biorxiv_medrxiv/biorxiv_medrxiv/pdf_json data set.

## Highlight:
* A search engine specially built for the CORD dataset
* Whole dataset and search result analysis, clustering and visualization 

## Algorithms/Method Used:
* Ranking: BM25 Okapi
* Clustering: PCA & t-SNE & K-means
* Topic Model: LDA
* Text Preprocessing: Language Filtering, Stopwords, Stemming, Vectorization
 <img width="601" alt="Screen Shot 2021-03-10 at 10 10 44" src="https://user-images.githubusercontent.com/63271980/110650645-bb217700-8188-11eb-9563-fd2cdf2b10f9.png">

## Usage:
command line: cd (absolute path of the folder "cs525project")->python3 manage.py runserver->broswer url:http://127.0.0.1:8000/mysearch

## Possible errors:
* python import error->Solution: pip3 install (missing package)
* file not found error->Solution: change absolute file path of the databse file and image src in the code
