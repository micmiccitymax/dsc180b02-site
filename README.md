# Finding Commonalities in Misinformative Statements Across Topics
## What Data Are We Using?
<img src="/assets/img/Snopes.png"> 
<img src="/assets/img/inforwars.png">
<img src="/assets/img/polifact.png">
Our data is collected from http://fakenews.research.sfu.ca/#parseWebs where we use the datasets containing Snopes, Politifact, and Emergent.info articles of varying real and fake news from 2010 to 2018. We took articles from each dataset to create a new dataset that contains real and fake news for specific genres of news. We gathered news about 100 data for each political and scientific topic from the Snopes, Politifact, and Emergent.info datasets to use as our training dataset. We also created a dataset filled with varying topics to use as our testing dataset The data included in this set is a mix of recent informative and misinformative articles. Our plan with these datasets is to find commonalities of misinformation across different topics. To do this, we are training our models based on set genres and then testing the results to a set of data with varying genres of news. 
## What are we trying to predict
For our research, we are using our training dataset to predict whether a random article, regardless of the genre, is misinformative or not. We will train our models so that it learns the commonalities of misinformation for a set topic. Then we will test our findings onto a random article to see if our model can accurately predict whether that article is misinformative or not. We use the scores of the Decision Tree, Naive Bayes, Logistic Regression, Random Forest Classifier, Stacking Model, and SVM to test our models’ accuracies. After our models make a prediction on a random genre article, we want to examine differences of misinformation across different genres of news.
## What models are we using for prediction
### Decision Tree
<img src="/assets/img/decision_tree_example.png">

### Logistic Regression
<img src="/assets/img/logistic_regression_example.png">

### Random Forest Classifier
<img src="/assets/img/random_forest_classifier.png">

### SVM
<img src="/assets/img/svm_example.png">

### Data Analysis
<img src="/assets/img/science_logisitic_cloud (1).png"> 
Fig 1: Word Cloud of Most Important Words for Science Articles

<img src="/assets/img/economics_logisitic_cloud (1).png">
Fig 2: Word Cloud of Most Important Words for Economic Articles

<img src="/assets/img/politics_logisitic_cloud.png">
Fig 3: Word Cloud of Most Important Words for Politic Articles

<img src="/assets/img/general_logisitic_cloud.png">
Fig 4: Word Cloud of Most Important Words for All Above Article Topics

## Results and Conclusions
### Accuracy Percision and Recall

### Commonalities

## Works Cited
