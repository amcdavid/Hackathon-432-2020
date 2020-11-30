# 432 2020 Test Predictions

The datasets you are predicting on will be found under the Box link containing the project data.  Unzip them and then run your prediction pipeline.

# Logistics

1.  Predictions on test data set are submitting by uploading the Box folder with your initials.  You should have received an email invite to this folder.  Under this folder, place your prediction as set of files named predictions should be named [<Date String><Ignored>.csv](prediction/01Dec2020-A.csv).  `<Date String>` should match the folder name, and everything else after this will be used as a label, ie, if you are providing predictions for more than one algorithm or data processing modality.
2.  Predictions will be scored at least once daily, with scores posted by noon on 3-December.  You may provide predictions for both recently uploaded data, as well as previous datasets.
3.  The scoreboard is located
    [here](https://amcdavid.github.io/Hackathon-432-2020/Leaderboard.html), and will be updated starting noon on 3-December.  I cannot provide support beyond the messages indicated on the Leaderboard if there are errors
    encountered in scoring your predictions.
4.  Final scoring will be done no earlier than 11:59PM 15-December.  You must provide at least one set of predictions for both of the two classifiers to get credit for this portion of the project.

# Prediction formats

*  Your predictions should be provided as a tab separated file with one header line
*  It must be in the same order as the `Alias` and `visit_num` provided in the test data `illness_control.tsv` file -- no join is performed
*  It must include a numeric column named `prediction`. Other columns can be included but will be ignored. Larger numeric values will be taken to mean more confidence in `is_illness==TRUE`, ie, if you want to provide only a binary classification then you can code no illness as 0 and yes illness as 1, or if your classifier provides probabilities, you can just provide the probability of illness here.  [See example predictions](prediction/01Dec2020-A.tsv)

