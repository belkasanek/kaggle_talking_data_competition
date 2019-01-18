# [Kaggle TalkingData Competition](https://www.kaggle.com/c/talkingdata-adtracking-fraud-detection)
 The task was about to predict whether a user will download an mobile application after clicking a mobile application advertisement. It's actually fraud detection task, they want to know which clicks are relevant. There are just 7 columns: ip, app_name, device, os, channel and click time, but train and test set contains about 250 millions of rows. Submissions are evaluated on area under the ROC curve between the predicted probability and the observed target.
 
 10 fold stack of solution above gives me following scores on public and private leaderboard.
|public score|private score|final rank| 
|---|---|---|
|0.9804|0.9820| 56th (*top2%*)|
