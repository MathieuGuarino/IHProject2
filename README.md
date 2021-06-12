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
The dataset come from :
[Compiled datasets for CDP Analytics Competition](https://www.kaggle.com/seraphimstreets/environmentequity-starterpack)

There is a lot of files so I needed to check first which file could be interesting, clean it up then merge it with other data

<a name="workflow"></a>

## Workflow
The first difficulty was to choose a direction and to filter the non necessary data. Indeed there is a huge number of file for a short period of time.
Even with a few files that was a lot of data in the columns so I needed to filter.
The dataset selected are : Fossil Fuel Prices (1989-2019), Percentage of Energy Consumption by Country, CO2 emissions by country, Pollution emissions by region, Deaths by Particulate Matter Air Pollution vs PM25 by country, Green Growth Indicators by country.
My first step was to host the datasets on google drive.
The second step was to merge and clean 4 of these datasets. The other 2 are used as secondary information.
The third step was to analyze data with correlation, plots, heatmap, histograms
The fourth step was to use PCA to compare countries
Then we 
<a name="organization"></a>

## Organization
How did you organize yourself? Did you use any tools?

<a name="links"></a>

## Links
Include the links to your repository, slides and trello. Feel free to include any other links associated to your project. 

[Repository](https://github.com/screamzz/IHProject2/)   
[Slides](https://docs.google.com/presentation/d/1DR6nLEWwSqqzdO_rTZZ4NDeUlRWxGYmABaZnsvkvd6Q/edit?usp=sharing)

# Conclusion

We can see that the energy consumption and production is changing over the years.
Some countries have a defined pattern with energy and look alike with some others.
There is clearly a link between PM25 and deaths by pollution.

# Going further

I spent a lot of time selecting data, and it's still not enough to dig through it.
The other files are also interesting to see if we can link more data and discover new patterns.
For speed I cleaned and removed a lot of data from some datasets because I needed to bind data from the same year, but the removed data is still interesting, for example I saw two falls in CO2 and production around 1914-1918 and 1939-1945 which are probably linked with the two wold wars.