# Vaccine_Project

Eli Ingleson and Imani Thompson

# Business Problem

Recently, a community outreach program has reached out to us. They want to increase the number of people properly vaccinated in their community. They want a model to determine whether or not an individual has or has not been vaccinated against the seasonal flu. This will help keep people healthy and keep hospitals from being as full from both flu and COVID-19 patients.

# About the Data

We got our data from the National 2009 H1N1 Flu Survey. This data was sponsored by the CDC and was originally used to produce estimates of vaccination coverage rates across the United States.

 The original data had 26,000 columns and 36 columns; however, we ended up only using 18 columns. The data had information about H1N1 and seasonal flu vaccines, sex, race, education, and many other factors.

# Methods

Our original data had information about H1N1 vaccines as well as seasonal flu vaccines. Since our employers only asked us to deal with seasonal flu data, we immediatly dropped all of the columns pertaining to H1N1 vaccines.

Furthermore, we also dropped several survey response columns as well. For instance, there were columns asking if a person was worried about getting the flu or not. Another one asked respondents if they had avoided large groups to stay healthy, but what exactly constitutes a large group? Because these columns were not strictly objective with their information, we dropped them as well.

# Modeling

We began our modeling with a model-less baseline. We found that our data was very balanced between people who had received vaccines and those who had not. This led us to choose accuracy as our primary metric.

Next, we created a variety of baseline models. We had a KNN model, a decision tree, a naive bayes, and a logistic regression model. After seeing that our decision tree was performing the best, we tuned its hyperparameters to increase our accuracy.

# Final Model

Our final model was a decision tree we ran a gridsearch on. With our best parameters for this model, we can predict whether or not an individual has received their flu vaccine with 75% certainty.

# Conclusion

According to our final model, we can determine if someone got their seasonal flu vaccine with 75% accuracy. Furthermore, in our data, we found several trends that could be useful to our employers. For instance, we found people with lower incomes were less likely to get vaccines, while older people and educated people were more likely to.

With this knowledge in mind, we would recommend our employers to advertise to middle-aged people and to make flu shots more available in low income areas.

This project was fascinating, and if we had had more time in the project, we would have taken some certain steps next. First, we would like to find a way to decrease the number of false positives in our model. This would reduce the number of people we think were vaccinated but actually are not.

We would also like to experiment with different feature combinations to see if we could create a better model. The last thing we would like to do is find a "convinceable target."

Some people will get a vaccine without any encourgament. Some will never get a vaccine despite how much encouragement they receive. However, there is a population that will get their vaccine with encouragement that would not without that help. By finding what charateristics make up this population or 'convinceable target', we can reach out to them and have more people be vaccinated. 

# Repo Navigation

├── Notebooks        <- Working notebooks.  
├── License          
├── Final Notebook   <- Report Notebook         
├── README.md        <- The top-level README for developers using this project.