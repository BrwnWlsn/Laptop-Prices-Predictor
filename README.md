# Laptop Prices Predictor
<ul>
  <li>Designed a web app that predicts the price of the laptop given the configurations. </li>
  <li>Scraped the laptops data from https://github.com/BrwnWlsn/Laptop-Prices-Predictor/releases using python and BeautifulSoup package</li>
  <li>Developed Linear, Lasso, and Random Forest Regressors using GridsearchCV to get the best model.</li>
  <li>Deployed the Machine Learning model using streamlit library in Heroku using flask</li>
</ul>

# Links and Resources Used
<li>PyCaret Library: <a href="https://github.com/BrwnWlsn/Laptop-Prices-Predictor/releases">https://github.com/BrwnWlsn/Laptop-Prices-Predictor/releases</a></li>
<li>Streamlit Library: <a href="https://github.com/BrwnWlsn/Laptop-Prices-Predictor/releases">https://github.com/BrwnWlsn/Laptop-Prices-Predictor/releases</a>
<li>Model Deployment Video: <a href="https://github.com/BrwnWlsn/Laptop-Prices-Predictor/releases">https://github.com/BrwnWlsn/Laptop-Prices-Predictor/releases</a></li>
<li>Model Deployment Github: <a href="https://github.com/BrwnWlsn/Laptop-Prices-Predictor/releases">https://github.com/BrwnWlsn/Laptop-Prices-Predictor/releases</a></li>
<li>Packages: pandas, numpy, sklearn, flask, streamlit, joblib</li>

# Web Scraping

This is the Flipkart website comprising of different laptops. This page contains the specifications of 24 laptops. So now looking at this, we try to extract the different features of the laptops such as:
<ul>
  <li> Description</li>
  <li>Processor</li>
  <li>RAM</li>
  <li>Storage</li>
  <li>Display</li>
  <li>Warranty</li>
  <li>Price</li>
</ul>
So we extract the data from 7 pages so our dataset now consists of the information the 168 different laptops. <br>
Link to my article: https://github.com/BrwnWlsn/Laptop-Prices-Predictor/releases

# Feature Engineering
We go through all the features one by one and keep adding new features. I have made the following changes and created new variables:
RAM - Made columns for Ram Capacity in GB and the DDR version <br>
Processor - Made columns for Name of the Processor, Type of the Processor, Generation <br>
Operating System - Parsed the Operating System from this column and made a new column <br>
Storage - Made new columns for the type of Disk Drive and the capacity of the Disk Drive <br>
Display - Made new columns for the size of the laptop(in inches) and touchscreen <br>
Description - Made new columns for the company and graphic card <br>

# Data Preprocessing
There are a few columns which are categorical here but they actually contain numerical https://github.com/BrwnWlsn/Laptop-Prices-Predictor/releases we need to convert few categorical columns to numerical columns. These are DDR_Version,Generation,Storage_GB,Price.

# Exploratory Data Analysis
![](https://github.com/BrwnWlsn/Laptop-Prices-Predictor/releases)   ![](https://github.com/BrwnWlsn/Laptop-Prices-Predictor/releases) <br/>
![](https://github.com/BrwnWlsn/Laptop-Prices-Predictor/releases)

# Model Building
<li>Traditional Method</li>
Used scikit-learn library for the Machine Learning tasks. Applied label encoding and converted the categorical variables into numerical https://github.com/BrwnWlsn/Laptop-Prices-Predictor/releases I splited the data into training and test sets with a test size of 20%. I tried three different models ( Linear Regression, Random Forest Regression, XGBoost) and evaluated them using Mean Absolute Error. 

<li>Automated Method</li>
Used the auto ML library in python called PyCaret. Compared all the regression models and selected the best model for applied hyperparameter tuning and plotted the various curves.

Link to my article: <a href="https://github.com/BrwnWlsn/Laptop-Prices-Predictor/releases">https://github.com/BrwnWlsn/Laptop-Prices-Predictor/releases</a>

# Model Deployment
I have deployed the model using Streamlit library and flask framework on Heroku which is a Platform As A Service(PAAS)
![](https://github.com/BrwnWlsn/Laptop-Prices-Predictor/releases)
![](https://github.com/BrwnWlsn/Laptop-Prices-Predictor/releases)

Web application: <a href="https://github.com/BrwnWlsn/Laptop-Prices-Predictor/releases">https://github.com/BrwnWlsn/Laptop-Prices-Predictor/releases</a>
