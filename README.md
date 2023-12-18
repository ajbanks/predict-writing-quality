# predict-writing-quality

Business Logic
Given a dataset of essays graded by expert human annotators, develop a deep learning model to analyze
and predict the quality of an essay. The quality of an essay is affected by such factors as topic relevance,
organization and coherence, word usage, sentence complexity, grammar and mechanics.

Datasets
"train.csv" - data used to train the model
"test.csv" – data used for prediction
"submissions.csv" – populate this file with the results
"submission_sample.csv" – sample reference of the submission data file
Schema
Name Type Description
id integer Unique ID corresponding to the essay
content string Content of the essay
output int Whether quality is high or low (1 or 0)


Predictive Modeling and Model Evaluation
Build a neural network that predicts the quality of an essay.
Experiment with different preprocessing methods, number of layers, types of layers, activation functions,
and any other relevant parameters. Compile the model by specifying the loss function and optimizer. Ensure
that the model is not overfitting.

Assess model performance on "train.csv" using the "Accuracy“ metric. Information about the metric is here.
The model will be tested on a different dataset from training to test its robustness.

Submission
For each record in the test set (test.csv), predict the value of the 'output' variable. Submit a CSV file with a
header row and one row per test entry. The file (submissions.csv) should have exactly 2 columns:
id
output (0/1)

Test Evaluation
The score will be automatically evaluated based on the value of the Accuracy metric for the
“submissions.csv” file. Get the best possible value of the metric during model development. The reviewer
might dive deeper into the Jupyter notebook to get more context.
