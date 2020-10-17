# Covid-19
Models of pre and after lockdown spread of Covid-19 in the UK.

I have analysed one of the dataset available on Kaggle regarding the spread of Covid-19 in England.



(https://www.kaggle.com/roche-data-science-coalition/uncover/tasks?taskId=1064)

 

csv:   covid-19-uk-historical-data.csv



The blue and the red line mark the date of the lockdown and 5 days later , the incubation period for Covid-19.



I have used sci-kit learn to fit a linear model on the two portions of the dataset (pre and after the lockdown) assuming an exponential progression and a linear one in the two cases. 
