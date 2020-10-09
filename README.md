I've been toying around with this <a href='https://www.kaggle.com/anmolkumar/health-insurance-cross-sell-prediction' >dataset</a>, trying to get the best prediction. There were quite a few issues including imbalanced classes with only about 12% positives. <br>
Also even when I got AUC around 85-86%% the F1 score was miserable, just under 1%, because the models were not capable to predict True Positives. <br>
Then I noticed that quite a few notebooks posted there were getting insane scores hitting over 95%. I was puzzled at first, but after analyzing the codes I understood that all of these notebooks had the same error - target leak.<br>
So I created this very simple notebook giving an example of how to avoid this mistake by creating clean validation/test set before doing any type of oversampling.<br>
Of course this is the most obvious way to get the target leak, but it is most often occuring too.
