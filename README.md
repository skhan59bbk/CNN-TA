# msc-data-science-project-2020_21---files-skhan59bbk

----------------------------------------------------------------------------

### Title: A Deep Learning Approach to Evaluating Technical Analysis of Financial Markets

This repository contains all the code written for my final MSc project. All code is written in Python (v3.7 and above) and the files here are either .py or .ipynb format. Google Colab was used to build and run the one .ipynb file. For all other files, there is a requirements.txt file included in this repo with a list of packages used.
I was awarded a Distinction for this project (and for the Masters overall).

A brief explanation of the files is provided below:

- eda.py

This was used for exploratory data analysis on the S&P500 index and its constituents, looking at things like volatility, correlations and distributions of returns. Also retrieves latest list of S&P 500 constituents and exports to 'spx-tickers.csv' file for reference.

- correlations.py

Another data analysis file, focusing specifically on returns correlations between the stocks. Conducts some web scraping from Wikipedia and creates the Minimum Spanning Trees.

- correlations-notebook.ipynb

The same as correlations.py but as a Colab notebook (building the MST required the help of a GPU).

- candlesticks.py

This is where the chart image generation process takes place. Technical indicators were calculated, forecast windows and labelling  added, and charts were saved.

- cnn-model-development.ipynb

The main Colab file where the model was built and evaluated. Includes data preprocessing steps. 

#### Data
The original dataset is too large to add to this repository, but is available from https://www.kaggle.com/alexsumt/stock-ohlc-data-sp500 

The final dataset of images (and/or the equivalent numpy arrays) are available on request - though also large in size. 
