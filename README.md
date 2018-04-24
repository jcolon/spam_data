# spam_data
Spam Filter <br><br>
You can create a Naive Bayes Classifier to filter the spam emails by following steps:
1. Load the spam dataset by clicking the "Open file..." button.
2. Select different attributes, and review the information in the right section.
3. Remove the capital_run_length_average, capital_run_length_longest, and capital_run_length_total attributes.
4. The remaining attributes represent relative frequencies (Numeric type) of various salient words and characters in emails. We will convert these to Boolean values (Nominal type) instead. To do this, click Choose button in the Filter frame and pick filters -> unsupervised -> attribute -> NumericToBinary. By clicking Apply button, all the numeric attributes are converted to Booleans. Each email is now represented by a 55 dimensional vector representing whether or not a particular word exists in an email.
5. You can save this filtered dataset to a new file by clicking Save... button.
6. Go to the Classify tab and click Choose button, then select the naive bayes model under classifiers -> bayes -> NaiveBayes.
7. Use Percentage split and leave the default settings, then click Start to build the classifier. Study the result in the right section, most importantly the percentages of correctly and incorrectly classified instance.
8. Examine the classifier models produced by WEKA.
9. Next, we would classify a test data by using this classifier. Download the spam_test.arff. Under the Classify tab, select supplied test set and load the test file by clicking "Set..." -> "Open file...". Finally, run the Naive Bayes Classifier on this test set.
