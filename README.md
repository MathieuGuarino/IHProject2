# Is there a link between how a country consume energy and health ?
# How is changing energy consumption and production over the years ?
*Mathieu Guarino*

*[Iron Hack, DataAnalyze & 12/06/2021]*

## Content
- [Project Description](#project-description)
- [Hypotheses / Questions](#hypotheses-/-questions)
- [Dataset](#dataset)
- [Workflow](#workflow)
- [Organization](#organization)
- [Links](#links)

<a name="project-description"></a>

## Project Description
There are several dataset with energy production/consumption, PM2.5 pollution, gas emissions, population, deaths by air pollution. The goal is to clean a linked all these datasets to find if there is any correlation in the data. The datasets are hosted on google drive and I will use Pandas, seaborn and matplotlib, stats to analyse the data.

<a name="hypotheses-/-questions"></a>

## Hypotheses / Questions
Is there a link between how a country consume energy and health ?
How is this behavior over the years ?
Is the CO2 / PM25 linked with the country population size ?
Is the behavior better over the years with renewable energies ?
What is the most used energy ?
Who is consumming the most over the wolrd ?

<a name="dataset"></a>

## Dataset
There is two data sources :
The Global Health Organisation API

Kaggle CSV files Dataset :


I accessed Kaggle by creating a account on the website to download the files. The GHO is open and I read the documentation of the GHO OData API.

I cleaned the data with pandas then uploaded it with mysql.connector on SQL Cloud. I then accessed merged data with mysql.connector and SQL Queries

[Dataset](https://www.kaggle.com/imdevskp/malaria-dataset) 
[GHO API](https://www.who.int/data/gho/info/gho-odata-api)

<a name="workflow"></a>

## Workflow
The first difficulty was to find data which can be linked on the topic of Health.
I found the GHO API which has data on doctors by country. The only problem was that the country information was using short names so I had to get the country full name with another request then clean the data.
The dataset has malaria information by country.
My first step was to get these data and clean them into dataframes ready to be transfered into two SQL tables.
My second step was to learn how tu use cloud SQL with python and I followed a tutorial and some documentation after creating a test account on Google.
The third step was to cast the data into the right format and create the SQL tables. I had problems with numpy datatype.
The last steps was getting merged data from the two tables into python dataframe then do some stats to show if the number of sick people is only linked with the number of doctors.

<a name="organization"></a>

## Organization
How did you organize yourself? Did you use any tools?

<a name="links"></a>

## Links
Include the links to your repository, slides and trello. Feel free to include any other links associated to your project. 

[Repository](https://github.com/screamzz/DataSets-SQL-API/)  
[Trello](https://trello.com/b/9HULHhAJ/iron-hack)  

