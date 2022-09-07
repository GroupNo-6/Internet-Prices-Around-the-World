# Internet-Prices-Around-the-World

 ### All the csv files used for the project are located in the [Resources folder](/Resources)
 ### The jupyter notebook used for cleaning, tranforming and loading is located in the [Main folder](InternetPricesWorldWide_Notebook.ipynb)

## Table of Contents

* [Teammates](#team-memebers)
* [Purpose](#purpose)



## Team Memebers: 
For this project, we've teamed up for the ELT process, we are:

* Hassan Mohamed
* David Nguyen
* Hwa Hara
* Joshua Cressaty
* Hector Custodio
* Maheen Abdulwaheed


## Purpose: 
 The main goal of this project is to perform the ETL process (Extract, Transform, Load) and document our steps taken in the process. The steps includes documenting the datasets used and their sources, types of data wragnling perfomed like cleaning, joining, filtering and aggregating. Also, the schemata used in the final production database.  The data for the extraction process can come from many different sources such as csv files, json files, html files, sql databases or spreadsheets. In this project , we've used 4 different csv files for extraction. We have jupyter notebook to transform the data. The transformation process includes data cleaning, selecting, joining , filtering and aggregating the data that we've used. For loading the data , we've used PostgreSql. 

 In this project we've used 4 different datasets to examine the different characteristics of different countries' internet speed and price. Some countries will have faster internet speed and more users due to the availability of advanced technology, but some countries will have significantly fewer users and slower speed due to limited access to technology. Our group would like to explore these characteristics in one dataset table.

 [Image](/Internet-Prices-Around-the-World/Images/ForREADMe.png)

 ## Extraction:

 For this project we explored many Datasets that were available on this [Kaggle website](https://www.kaggle.com). We were able to find the following:

 * [data set](https://www.kaggle.com/datasets/ramjasmaurya/1-gb-internet-price) : This contains a dataset of internet prices around many countries and islands. 
 * [data set](https://www.kaggle.com/datasets/prasertk/internet-broadband-and-mobile-speeds-by-country) : This contains Internet broadband speed by country.
 * [data set](https://www.kaggle.com/datasets/cityapiio/world-cities-average-internet-prices-2020) : This contains the world cities average USD internet prices.
 * [data set](https://www.kaggle.com/datasets/sansuthi/gapminder-internet) : this contains the Internet Usage rate per 100 people population.

 We were able to read all the above CSV files using jupyter notebook and importing pandas as pd. 


 ## Transform :
 
 After cleaning, merging and renaming columns in our comibned final dataframe. We Were left with the following columns:

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





  




 





