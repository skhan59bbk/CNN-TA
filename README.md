This repository contains all the code written for my final MSc project, for which I received a Distinction.


----------------------------------------------------------------------------

### A Deep Learning Approach to Evaluating Technical Analysis of Financial Markets

Financial market traders have long poured over stock charts, looking for repeatable patterns or indicator readings that may precede profitable moves in price. While many of the techniques can be formalised and tested empirically, much of technical chart analysis is still subjective and in the eye of the practitioner. Advances in deep machine learning, specifically in Computer Vision, have opened the door to new ways of testing these pattern recognition exercises. This project explores financial market forecasting using nothing more than stock charts to see if deep learning models can “see” what some traders see, classifying these images as bullish or bearish based on their short-term future price returns. The results are intriguing and surpass expectation, suggesting there may well be some utility in technical analysis – at least when carried out by a convolutional neural network.


----------------------------------------------------------------------------

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
