# Milestone P3


## Title : Predicting covid cases with Google Trends

### Abstract
Since January 2020, the covid-19 pandemic has challenged the various hospital systems. The response to this health crisis has often been a lockdown, causing an economic and social crisis. This response is in reaction rather than in preparation and anticipation.

Since the situation evolves every week, it's interesting to have an accurate short term forecast in order to better anticipate the next outbreak and develop a better strategy to contain the virus and thus limit the economic and social impact. This study proposes to extend the method used in the paper “Predicting the present with Google trends” to develop a short term forecast of the number of Covid-19 cases in France. Then, improving this prediction using appropriate and relevant Google Trends data. For example, by including indexes of topics related to health at the level of research on the symptoms of Covid, or by using indexes related to social life and which could indicate an increase in trips and gatherings over a given period.

### Research Questions

1.  What topics are mostly related to the evolution of the number of cases in France?
    
2.  Does including the indexes related to health (symptoms, cough...) to our model improve our forecast?
    
3.  Given the many restrictions around social life applied during this pandemic, it is interesting to wonder if including Google trends indices related to social life such as dining out in the summer period of 2020, could improve the prediction?
    
4.  Can Google Trends Data help to predict noisy data as Covid cases?
    

### Proposed dataset
 
1. **Official numbers of covid cases**
The [dataset](https://opendata.ecdc.europa.eu/covid19/casedistribution/csv) can be found on the EU open data portal. The dataset provides daily cases and deaths per country. We can therefore easily extract the daily cases for France.

2. Google trends indexes related to covid
Data can be downloaded as CSV files containing a timestamp and the corresponding index using [Google Trends](https://trends.google.com/trends/?geo=US).

For example : [Symptomes covid](https://trends.google.fr/trends/explore?q=symptomes%20covid&geo=FR) and [restaurant](https://trends.google.fr/trends/explore?geo=FR&q=Top%2010%20restaurant) indexes.


### Methods
    

1.  Collect the data
    
2.  Build the dataset
    
3.  Data pre-processing
    
4.  Apply the method of the Paper :
    

	- Fit an AR-1 model on the number of Covid cases in France time-series.

	- Discuss if we go for an in-sample or out-sample forecasting, the windowing, etc

	- Add the relevant indices to the model and redo the forecasting

5.  Evaluate the method
In term of MAE (Quality of prediction)

6. Discuss the Results
    
7.  Propose improvements

8. Report and Video
    
### Proposed timeline
- By the **2nd of December** : Step 1 to Step 3
- By the **9th of December** : Step 4 and 5
- By the **14th of December** : Step 6 and 7
- By the **18th of December** : Step 8
    
### Organization within the team

To respect our internal milestones, we propose the following organization within our team. Some tasks are not yet perfectly clear. Finally, close collaboration and good communication within the team will help us to do a successful project.

![Organisation within the team](https://github.com/epfl-ada/ada-2020-project-milestone-p3-data-y-nada-mas-1/blob/main/orga.png)

### Questions for TAs (optional)
We'd like to have your inputs on the use of Gtrends library. Since we are just willing to use the indexes without comparing, is it relevant to use as an extractor ? Or can we just download the csv files from google trends?
