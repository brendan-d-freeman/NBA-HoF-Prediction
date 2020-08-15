# NBA-HoF-Prediction

This repo includes the data necessary and notebook necessary to run the predictions for who in the current NBA has met the criteria to become a Hall of Famer based on historical records. The noetbook needs the following packages installed:
- Pandas
- Beatiful Soup
- Numpy
- Matplotlib
- Scikit-learn


The initial data set found with the repo is the [NBA Players stats since 1950](https://www.kaggle.com/drgilermo/nba-players-stats#Seasons_Stats.csv) found on Kaggle which is a consolidated dataset scraped from Basketball-Reference. The data is then enhanced with data scraped to provide how many championships a player won. how many All-Star games they were voted to, how many All-NBA teams they made, and how many MVP awards they won.

As you'll see in the notebook, the first approach I tried was using traditional classification models. However, HoFers are so unique amongst the total of NBA players that they are more considered anomalies. The approach that worked best then was to use models like One Class SVM and Isolation Forest that are designed specifically for anomaly detection.