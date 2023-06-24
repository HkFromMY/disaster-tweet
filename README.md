# Background

Twitter has become an important communication channel in times of emergency. The ubiquitousness of smartphones enables people to announce an emergency they’re observing in real-time. Because of this, more agencies are interested in programatically monitoring Twitter (i.e. disaster relief organizations and news agencies).

# Dataset Used
Each sample in the train and test set has the following information:
- The `text` of a tweet.
- A `keyword` from that tweet (although this may be blank)
- The `location` the tweet was sent from (may also be blank)
- The `target` whether the tweet is about a real disaster or not, `1` means Yes, `0` means No.

**Files:**
1. **train.csv** - the training set
2. **test.csv** - the test set
3. **sample_submission.csv**  - a sample submission file in the correct format

# Approach Used
1. Simple pre-processing & feature engineering
2. Uses pre-built BERT classification models from `simpletransformers`
3. Build own classification model with pre-trained BERT as feature extractor from Tensorflow Hub.
4. Choose the best model with highest score.
