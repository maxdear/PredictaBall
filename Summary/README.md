# Summary

## Data Frame Formation
Once all the data was collect it had to be sorted and merged into the match data frame, allowing a team's league table standings and their ELO ranking to act as predictors for a match's outcome. 

[shown here](https://github.com/maxdear/PredictaBall/blob/master/Notebooks/3.%20Data%20Merging.ipynb)

## Modelling
Before running a model, another predictor was created using a team's recent performaces to give a sense of form.
A Class was created to make this predictor as it used a team's points procured over various time frames multiplied by a weighting; making this a class allowed for the step to be included in the pipeline and the weightings to be grid searched as hyperparameters.
The [Modelling Notebook](https://github.com/maxdear/PredictaBall/blob/master/Notebooks/4.%20Modelling.ipynb) shows this work along with the pipelines of the various models that were tested.


## Results
Whilst the accuracy of the models were important, they could also be ranked on another metric; Profit and Loss. Having kept the bookies odds for each match in the data frame, a funciton was created to determine the profit and loss made by each model from betting equally on it's predictions. Whilst the likelyhood of any of the models making a large profit was slim over a relatively small data set, it was interesting to see how similarly accurate models differed in their betting results. 
The [Results & Profit-Loss Notebook](https://github.com/maxdear/PredictaBall/blob/master/Notebooks/5.%20Results%20%26%20Profit-Loss.ipynb) 
shows this in detail.

## Conclusion and Future Work
Although that none of my models proved to be consistently profitable, I was definitley moving in the right direction. I feel that in order to create an algorithim that is truly profitable, the next step would be determining how much to bet on certain matches and even when not to bet. The idea of betting equally on each match was good for academic purposes as it allowed a percentage return to be easily calculated however, in the real world one must capatalize on the sure things and avoid the undeterminable.

Having completed the project, there is one thing that I would have done differently. Use more data. Initially I thought that only fairly recent matches were relevant in predicting future matches however since most of the predictions relied on pure numerical data I now believe that the data set could have been made far larger by using multiple previous seasons. 

One tip I would give to anyone working on a similar project is to let the results show you what is a good predictor rather than choosing yourself. Initially I thought that a Team's name and their recent form would be the best indicators of a win, draw or loss but I soon came to realise that the models performed best when the team names were dropped and only a small influence of form was included. 
