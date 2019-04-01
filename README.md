# [Kaggle TalkingData Competition](https://www.kaggle.com/c/talkingdata-adtracking-fraud-detection)
 The task was about to predict whether a user will download an mobile application after clicking a mobile application advertisement. There are 7 columns: ip, app_name, device, os, channel and click time. Submissions are evaluated on area under the ROC curve between the predicted probability and the observed target. Train set + test set is about 250 million rows and except click time all features are categorial with high cardinality. Besides that the data is very unbalanced there is only 0.2% of positive class. Due to the size of data feature engineering had to be conservative. I used aggregation on various feature groups like count unique app for each ip, lag features, based on previous days values, ratios like number of clicks per ip. I trained and tuned LightGBM model using stratified 10 fold cross validation. Score of average prediction of these models is given below.

|public score|private score|final rank| 
|---|---|---|
|0.9804|0.9820| 56th (*top2%*)|
