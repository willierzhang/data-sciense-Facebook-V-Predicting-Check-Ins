# data-sciense-Facebook-V-Predicting-Check-Ins
In this competition we're given around 30 million (simulated) check-ins on Facebook in a 10km by 10km grid. 
The goal is to build a model that predicts what business a user checks into based on spatial and temporal information.
The tricky part here is that there are around 100k different classes(`place_id`) so most supervised learning techniques won't work on the entire dataset.
However most classes are clustered in only certain parts of the grid so the idea we will pursue here is to select a small-ish square within the grid and try to see 
if we can do better within the small square. First we will do some exploratory data analysis in the smaller square then we will use 
a random forest algorithm for prediction and finally, we will analyze the results.
