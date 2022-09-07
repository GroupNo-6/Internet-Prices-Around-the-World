# Internet-Prices-Around-the-World


## Table of Contents

* [Teammates](#team-memebers)
* [Purpose](#purpose)
* [Extraction](#extraction)
* [Tranformation](#transform)
* [Loading](#load)
* [References](#references)


## Team Memebers: 
For this project, we've teamed up for the ELT process, we are:

* Hassan Mohamed
* David Nguyen
* Hwa Hara
* Joshua Cressaty
* Hector Custodio
* Maheen Abdulwaheed


## Purpose: 
 The main goal of this project is to perform the ETL process (Extract, Transform, Load(into SQL or NoSQL Databse)) and document our steps taken in the process.  In this project , we've used Jupyter notebook for the ELT process. Pandas was used for reading and converting the CSV files. The transformation process included data cleaning, selecting, joining , filtering and aggregating the data that we've used. For loading the data into a datbase, we've used PostgreSql. 

 In this project we've used 4 different datasets to examine the different characteristics of different countries' and cities' internet speed and price. Some countries will have faster internet speed and more users due to the availability of advanced technology, but some countries will have significantly fewer users and slower speed due to limited access to technology. Our group would like to explore these characteristics in one dataset table.

 ![Image](/Images/ForREADMe.png)


 ## Extraction:

 For this project we explored many Datasets that were available on this [Kaggle website](https://www.kaggle.com). We were able to find the following:

 * [data set 1](https://www.kaggle.com/datasets/ramjasmaurya/1-gb-internet-price) : This contains a dataset of internet prices around many countries and islands. 
 * [data set 2](https://www.kaggle.com/datasets/prasertk/internet-broadband-and-mobile-speeds-by-country) : This contains a dataset of Internet broadband speed by country.
 * [data set 3](https://www.kaggle.com/datasets/cityapiio/world-cities-average-internet-prices-2020) : This contains the world cities average USD internet prices dataset.
 * [data set 4](https://www.kaggle.com/datasets/sansuthi/gapminder-internet) : this contains the Internet Usage rate per 100 people population dataset.

 We were able to read all the above CSV files using jupyter notebook and importing pandas as pd. We converted all of the above csv files into Dataframes. One of the Datasets read :

 ![Image](/Images/csv_read1.png)


 ## Transform :
 
 We were able to merge 3 of the above datasets together with no issues. We dropped the null values and some columns that we didnot need. The only problem we faced was to take quotaions out of the world cities average USD internet prices dataset. We were able to remove the quotations from the csv file and then added it back to our notebook for reading and converted it to a dataframe. We renamed it to cities_cleaned.csv and merged it to our final dataframe. After cleaning, merging and renaming columns, we came up with a comibned final dataframe. We were left with the following columns:

 * 'Country'
 * 'City'
 * 'Internet Price of City (USD)'
 * 'Average price of a GB in 2020'
 * 'Average price of a GB in 2021'
 * Average price of a GB in 2022'
 * 'Internet Plans Available'
 * 'Cheapest GB'
 * 'Most expensive GB'
 * 'Average National Internet Speed'
 * 'Internet users'
 * 'Internet Use Rate'
 * 'Broadband Mbps'

 A Screen shot of our Final Dataframe:

 ![Image](/Images/Final_Dataframe.png)

## Load:

The final DataFrame was converted into a CSV file and uploaded on Postgres by importing create_engine from sqlalchemy and importing pyscopg2. 


# References :

* For the images used in the project, we used it from this [website](https://images.search.yahoo.com/search/images;_ylt=AwrEtVcguBhjYaIScVpXNyoA;_ylu=Y29sbwNiZjEEcG9zAzEEdnRpZAMEc2VjA3BpdnM-?p=internet+around+the+worl&fr2=piv-web&type=E211US714G0&fr=mcafee#id=21&iurl=https%3A%2F%2Fstatic01.nyt.com%2Fimages%2F2019%2F03%2F07%2Ftechnology%2Finternet-cables-oceans-1552081048106%2Finternet-cables-oceans-1552081048106-facebookJumbo-v5.png&action=click)

* ### All the csv files used for the project are located in the [Resources folder](/Resources)
* ### The jupyter notebook used for cleaning, tranforming and loading is located in the [Main folder](InternetPricesWorldWide_Notebook.ipynb)



  




 





