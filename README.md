# Covid-19
### !!! NOTE: data at the beginning of the pandemic were not realiable at all! This is just an exercise to practise with data, machine learning and time series
### It is also important to note that the exponential model was not fit on training data. If there was more reliable data for a longer period of time I could have split the pre-lockdown-period in two chunks , let´s say 20 and 80% of the data each and check if an exponential model trained on the first 20% would fit the remaining 80% before diverging from the actual data due to the action of the lockdown measure. 


Models of pre and after lockdown spread of Covid-19 in the UK.

I have analysed one of the dataset available on Kaggle regarding the spread of Covid-19 in England.



(https://www.kaggle.com/roche-data-science-coalition/uncover/tasks?taskId=1064)

 

csv:   covid-19-uk-historical-data.csv



The blue and the red line mark the date of the lockdown and 5 days later , the incubation period for Covid-19.



I have used sci-kit learn to fit a linear model on the two portions of the dataset (pre and after the lockdown) assuming an exponential progression and a linear one in the two cases. 

The data refers to the period between the 30th of January 2020 to the 29th of July 2020 (180 days).


### !!! NOTE: data at the beginning of the pandemic were not realiable at all! This is just an exercise to practise with data, machine learning and time series
