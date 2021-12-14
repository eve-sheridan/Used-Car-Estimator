# Used-Car-Estimator
## A Big Data project using Craigslist Used Car Dataset to build a data science pipeline using Spark

### 1 Introduction
This project aims to build a real-world data science pipeline with Big Data tools such as Spark.  A typical machine learning (ML) project involves several processing steps including:
1.	Collecting data from one or more sources
2.	Exploratory Data Analysis (EDA), cleansing and wrangling
3.	Developing the ML pipeline, training and evaluating models
4.	Tuning the model for better performance and accuracy
5.	Deploying the ML model in production
6.	Monitoring the service and repeating the above steps when required

### 2 Project Motivation
Accurate car price prediction usually involves expert knowledge because price depends on many distinctive features and factors. Typically, the most significant factors affecting price are manufacturer and model, age, engine size and odometer reading.  However, there are many other factors that may influence price including type of fuel, exterior colours and type of transmission among others.  Determining which variables are significant in predicting the price of the car and how well those variables describe the price of the car is the goal of prediction tools.

There are a whole range of used car price guides available on the Internet such as carsales.com.au, RACQ or Drive to name a few.  Their prediction methods are usually not disclosed and their motivations for providing this information may vary from wanting to sell a certain model car to providing information for the public or increasing advertising revenue.  The prediction methods and motivations will influence the results provided.  There is a need for a used car price prediction system to effectively determine the worthiness of the car using a variety of features that is unbiased and based on data. 

Being able to predict a used car’s market value can help both buyers and sellers.  There are three target groups who could benefit from this prediction model.
-	Used car sellers or dealers could use this information to better understand what makes a car valuable and what the important features are to more accurately price their cars.  This will enable them to provide a better service to their customers and also increase their sales revenue.
-	Online pricing services would usually already have a prediction model but could benefit from looking at additional models to help improve their predictions.  Models may become less effective with time as outside influences can change what variables influence the vehicle price.
-	Individuals who are looking to buy or sell a vehicle would benefit greatly from knowing what the true market value of a vehicle is in order to be able to accurately price vehicles they list for sale and to avoid being overcharged when purchasing a new vehicle.

### 3 The Dataset
You can download the original file from the links below and save as vehicles.csv to your computer before running this code from the beginning.  Note this is quite a large file.

Alternatively, you can use the cleaned dataset provied 'vehiclesclean2.csv' and go directly to section 4 in the Jupyter Notebook

- Description:	Used Cars Dataset.  Vehicles listings from Craigslist.org
- Website URL: https://www.kaggle.com/austinreese/craigslist-carstrucks-data  
- Download File URL: https://www.kaggle.com/austinreese/craigslist-carstrucks-data/download 
- Note: access to this file is free but you need to set up an account with Kaggle in order to be able to download the file.
- Size:	Zipped download file: 165 MB; Extracted csv file: 1.35 GB
- Dimensions: 426,880 records, 26 attributes
- 26 attributes: 
['id',   'url',   'region',  'region_url',  'price',  'year',  'manufacturer',  'model',  'condition',  'cylinders',  'fuel',  'odometer',  'title_status',  'transmission',  'VIN',  'drive',  'size',  'type',  'paint_color',  'image_url',  'description',  'county',  'state',  'lat',  'long',  'posting_date']
- Owner	Austin Reese: https://www.kaggle.com/austinreese
- Updates:	Expected update frequency: Quarterly; Last updated: 2021-05-07; Date created: 2018-10-11; Current version: Version 10
- Date Range:	4th April 2021 – 4th May 2021



