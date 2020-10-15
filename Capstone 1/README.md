
# COVID -19 ANALYSIS AND PREDICTION 

![Image](https://github.com/umamohantm/springboard/blob/master/Capstone%201/Data/Covid.png)


# CONTEXT:


COVID-19 is an infectious disease caused by severe acute respiratory syndrome corona virus 2. It was first identified in December 2019 in Wuhan, Hubei China and resulted in an ongoing pandemic. As of 27 July 2020, more than 16.2 million cases have been reported across 188 countries and territories, resulting in more than 647,000 deaths. More than 9.36 million people have recovered. The virus is primarily spread between people during close contact, most often via small droplets produced by coughing, sneezing, and talking. Preventive measures include social distancing, washing hands with soap and water often, sanitizing frequently touched surfaces, wear a face mask, cover coughs and sneezes with a tissue, avoid sharing personal household items, etc,. Social distancing strategies aim to reduce contact of infected persons with large groups by closing schools and workplaces, restricting travel, and cancelling large public gatherings.


# This project deals with two sections.

1. First section includes the analysis of history of covid-19 in which countries this pandemic started and how many countries are affected till date, early stage of this pandemic versus today (August 9th, 2020), count of covid-19 infected during the period from December 31st, 2019 to August 9th, 2020, fatality of this pandemic, strictness of lockdown, population density of the countries because it plays a major role in this spread, hand washing facilities and sanitary facilities, hospital facilities , etc,. The data used in this project is a collection of the COVID-19 data maintained by Our World in Data. 

2. Second section deals with the prediction of total covid-19 infected people in the upcoming 10 days by considering the infected graph for the past few months. Here ARIMA model is used for predicting the covid-19 infected people count. 


# Approach
## This problem contains the following steps 
Data Collection : The data used in this project is a collection of the COVID-19 data maintained by Our World in Data. It is updated daily and includes data on confirmed cases, deaths, and testing, as well as other variables of potential interest. <br>
Data Wrangling : The data originally obtained was in CSV file and directly loaded into the pandas data frame . The NAN values are filled with forward fill, backward fill, with mean and median, and interpolate. <br>
Exploratory Data Analysis:This section involves the visualization part to know the insights from the dataset. <br>
Modelling :The approach used in this project is time series analysis and the model applied is ARIMA (Autoregressive Integrated Moving Average). The accuracy is measure using AIC (The Akaike Information Critera).<br>


# Results :<br>

### Actual Vs Predicted(India, August,2020)
![Image](https://github.com/umamohantm/springboard/blob/master/Capstone%201/Data/India_table.PNG)
The AIC value is 523.422.

Covid-19 has infected over 19 million people worldwide and claimed more than 721K lives with Europe, the United States, Brazil and India overtaking China where the pandemic started last December.<br>
The drastic outbreak spread is influenced by the countries various factors like strictness of lockdown, population density, hygiene and hand washing facilities, smoking population.<br>
COVID-19 is still an unclear infectious disease, which means we can only obtain an accurate ARIMA prediction after the outbreak ends.<br>


