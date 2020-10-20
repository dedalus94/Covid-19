# Covid-19 spread in the UK
#### Any conclusion from this work has no **scientific value**, I am not an epidemiologist or specialised in modelling the spread of infectious diseases. Other models better predict/analyse the spread of infectious diseases, such as the SIR model: https://en.wikipedia.org/wiki/Compartmental_models_in_epidemiology 

More on mathematical models in epidemiology:
https://www.ncbi.nlm.nih.gov/pmc/articles/PMC5348083/

Paper trying to explain the post-lockdown linear growths:
https://www.pnas.org/content/117/37/22684

This approach simply consists in assuming the same exponential growth observed during the first period of the epidemic to make predictions about an unmitigated spread of covid-19, and it is not correct. The exponential growth will only continue for a period of time which depends on, among other things, on RT.

## How to navigate the notebook, file sources, general ideas behind this work: 

I have analysed one of the dataset available on Kaggle regarding the spread of Covid-19 in England.

(https://www.kaggle.com/roche-data-science-coalition/uncover/tasks?taskId=1064)

csv file is:   covid-19-uk-historical-data.csv

The blue and the red vertical lines mark the date of the lockdown and 5 days later , roughly the incubation period for Covid-19.

I have used sci-kit learn to fit a linear model on the two portions of the dataset (pre and post-lockdown) assuming an exponential progression and a linear one in the two cases. 
In order to fit the linear model on the datapoints referring to an exponential growth of the epidemic, I have taken the logarithm of the datapoints and then I have exponentiated predictions of the model that I have fit on them. 

The data refers to the period between the 30th of January 2020 to the 29th of July 2020 (180 days).

## limitations, findings :

This notebook is meant to be an exercise for practicing with data analysis, Machine Learning, data visualisation and more aspects of Data Science / Machine Learning.

#### Any conclusions from this work have no **scientific value**. Other models better predict/analyse the spread of infectious diseases, such as the SIR model: https://en.wikipedia.org/wiki/Compartmental_models_in_epidemiology

The **data regarding the first period of the pandemic are highly unreliable** due to fewer tests and less awareness of governments/public around Covid-19. 


According to the model, cases were doubling every 5 days. it predicts 60 milion of infections by the 14th of May 2020, roughly the size of the British population.
If we take into account the SIR model and we assume an exponential growth for until only (roughly) half of the population has been infected, then by the 9th of May, or 47 days after the date of the lockdown enough people would have been infected to cause the death of hundreds of thousands dy the end of June 2020. 

My findings are that lockdown quickly and effectively stopped exponential growth of the pandemic, probably saving hundreds of thousands of people between April and June 2020. 

I could not find any correlation between masks being made compulsory on London´s public transport network and the the spread of the disease. 

It is hard to estimate the real effect of masks and disentangle it from the effect of social ditancing, changes in behaviour and other measures. 
Nevertheless it is also important to notice that when London emerged from the lockdown, with masks on public transport and in shops and with social distancing, the rate of spreading of covid-19 did not go back to the pre-lockdown exponential growth, but stayed linear.

I did not investigate other interventions due to lack of time. It would be interesting to repeat the analysis with the data from the second wave, mass testing will mean more robust and reliable data and a different range of approaches has been used in different areas of England over the last few months, unfortunately this dataset only covers the period between the end of January 2020 and the end of July 2020. 

## Comments are very appreciated. 


Update 20/10/20:

More on mathematical models:
https://www.ncbi.nlm.nih.gov/pmc/articles/PMC5348083/

Paper trying to explain the linear growth:
https://www.pnas.org/content/117/37/22684
