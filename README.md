# Milestone P3


## Title: Predicting covid cases with Google Trends

[Data story](https://covidtrends.github.io/)


### Abstract
Since January 2020, the covid-19 pandemic has challenged the various hospital systems. The response to this health crisis has often been a lockdown, causing an economic and social crisis. This response is in reaction rather than in preparation and anticipation.

Since the situation evolves every week, it's interesting to have an accurate short term forecast to better anticipate the next outbreak and develop a better strategy to contain the virus and thus limit the economic and social impact. This study proposes to extend the method used in the paper “Predicting the present with Google trends” to develop a short term forecast of the number of Covid-19 cases in France. Then, improving this prediction using appropriate and relevant Google Trends data. For example, by including indexes of topics related to health at the level of research on the symptoms of Covid, or by using indexes related to social life and which could indicate an increase in trips and gatherings over a given period.

### Research Questions

1. What topics are mostly related to the evolution of the number of deaths in France?
   
2. Does including the indexes related to health (symptoms, cough...) to our model improve our forecast?
   
3. Given the many restrictions around social life applied during this pandemic, it is interesting to wonder if including Google trends indices related to social life such as dining out in the summer period of 2020, could improve the prediction?
   
4. Can Google Trends Data help to predict noisy data as Covid deaths?  

### Proposed dataset
 
1. **Official numbers of covid cases**
The [dataset](https://opendata.ecdc.europa.eu/covid19/casedistribution/csv) can be found on the EU open data portal. The dataset provides daily cases and deaths per country. We can therefore easily extract the daily cases for France.

2. Google trends indexes related to covid
Data can be downloaded as CSV files containing a timestamp and the corresponding index using [Google Trends](https://trends.google.com/trends/?geo=US).

For example : [Symptomes covid](https://trends.google.fr/trends/explore?q=symptomes%20covid&geo=FR) and [restaurant](https://trends.google.fr/trends/explore?geo=FR&q=Top%2010%20restaurant) indexes.


### Methods
   

- 1 Data collection and pre-processing
 - 1.1 Collect of Covid-19 related data
	- 1.2 Pre-processing of Covid-19 related data
	- 1.3 Google Trends data (Create categories with associated key words)
      - 1.3.1 Categories with 10 key-words
      - 1.3.2 Extract google trends indexes

- 2 Cross-Correlation

- 3 Apply the method of the paper
	- 3.1 In sample predicition using AR-1
	- 3.2 Out-of-sample prediction

- 4 Conclusion

- 5 Going Further


### Proposed timeline
- By the **2nd of December** : Step 1 to Step 3
- By the **9th of December** : Step 4 and 5
- By the **14th of December** : Step 6 and 7
- By the **18th of December** : Step 8
   
### Organization within the team

To respect our internal milestones, we propose the following organization within our team. Finally, close collaboration and good communication within the team will help us to do a successful project.

![Organisation within the team](https://github.com/epfl-ada/ada-2020-project-milestone-p3-data-y-nada-mas-1/blob/main/orga.png)

### Repository structure
```
.
├── README.md
├── ada-project.ipynb
├── covid_cases.csv
└── orga.png
```

### Contributions

- Baudoin de Sury
- Mehdi Akeddar 
- Jérémy Plassman
