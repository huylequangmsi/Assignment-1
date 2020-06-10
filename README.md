# Assignment 1

Modern workflow in Data science - Assignment 1


## **1. Overview of the folder**

Assignment 1 folder consists of the following files: 

- **README.md**: presents the structure of the repository, the aim of the report, the dataset and a short analysis of results.

- **Codes.Rmd**: is an RMarkdown file, which stores the codes in R language detailing each steps of in downloading data, merging and cleaning data, and finally, ploting three graphs for analysis. Users just need to change the local drive in the beginning of this file, and run the codes to obtain the results shown here.


## **2. Introduction**

Coronavirus (Covid19) brings about a more severe crisis than almost any before. To protect people from the coronavirus, governments worldwide have had to implement safety measures that have a huge impact on personal and economic life. This report, however, does not aim at analyzing the consequences of Covid19, but to give an overview of the changes in the total of cases and infection rates over time (from January 2020 until June 2020). This report will zoom in the situation in some selected countries where coronavirus is more prevalent.

## **3. Data**

The dataset is taken from John Hopkins University (the JHU CSSE COVID-19 Dataset) which monitors the coronavirus epidemie situation all over the world and collects data on daily basis. The main data for analysis is the "Time_series_covid19_confirmed_global" showing the total of confirmed infected cases per country from 22 Jan 2020 until now. This dataset is then merged with the “UID_ISO_FIPS_LookUp_Table” to add some additional country characteristics variables (e.g. population, longitude, lattitude, country code, states...)

To download the datasets, just follow the steps in the Codes.Rmd.

## **4. Analysis**

First, Figure "Overall change" depicts an overview of the increase in the number of Covid19 infected cases all over the world. Each point in the line is the world average of the log number of confirmed cases at each point in time (daily). There is an increasing trend in the log number of cases, especially after March 2020, the number of cases have increased at a significant rate. 

![overall_change](https://user-images.githubusercontent.com/66418536/84247356-455c8200-ab08-11ea-8940-ef5deaf2f90e.png)

Figure "Change by country" zooms in 9 selected countries, namely, Brazil, China, Germany, Iran, Italy, Russia, Spain, United Kingdom, and United States. These countries are selected because they are currently having the highest number of infected people in the world. While the number of cases has been leveled off in China, Italy and Spain, it is still increasing very fast in the US, Brazil and Russia. Since the data is on daily basis, it shows a rather strange pattern in the UK, because the number of cases fluctuates strongly here, however, the overall trend is still going up.

![change_by_country](https://user-images.githubusercontent.com/66418536/84247489-789f1100-ab08-11ea-877b-8b8819238d6a.png)

Similarly, the last Figure "Infection rate" also zooms in these 9 selected countries. The infection rate is calculated by dividing the total of confirmed cases by the total population. To be easy to read, the infection rate is presented per 100,000 people. The US has the highest infection rate with almost 600 infected per 100,000 people, followed by Spain and Italy. However, the rate in Spain and Italy seems to stop increasing, meanwhile in the US, Brazil and Russia, there continues to be an increasing trend in the future. 

![infection_rate_graph](https://user-images.githubusercontent.com/66418536/84247544-8e143b00-ab08-11ea-8f9a-b926fcc04315.png)

Overall, both the number of cases as well as the infection rate have increased sharply since March 2020. Some countries have reacted quickly with strong measures such as Germany, Spain and Italy have seen a level off in the number of cases.
