<h1>Finding Commonalities in Misinformative Articles Across Topics</h1>
<h1>Link to our Github Repo! https://github.com/freebreadstix/capstone_B02</h1>
<h2>What Data Are We Using?</h2>
<p align="center"><img src="assets/img/Snopes.png">    <img src="assets/img/Polifact.png">     <img src="assets/img/emergent.jfif"> </p>

<p>Our data is collected from [Simon Fraser University's fake news research](http://fakenews.research.sfu.ca/#parseWebs) where we used the datasets containing Snopes, Politifact, and Emergent.info articles of varying real and fake news from 2010 to 2018. We took articles from each dataset to create a new dataset that contains real and fake news for specific genres of news. We gathered news about 100 data for each political and scientific topic from the Snopes, Politifact, and Emergent.info datasets to use as our training dataset. We also created a dataset filled with varying topics to use as our testing dataset The data included in this set is a mix of recent informative and misinformative articles. Our plan with these datasets is to find commonalities of misinformation across different topics. To do this, we are training our models based on set genres and then testing the results to a set of data with varying genres of news. </p>
<h2>What are we trying to predict</h2>
<p align="center"> <img src="assets/img/infowars.png"> </p>
 
<p>For our research, we are using our training dataset to predict whether a random article, regardless of the genre, is misinformative or not. After Preprocessing with TFIDF We will train our models so that it learns the commonalities of misinformation for a set topic. Then we will test our findings onto a random article to see if our model can accurately predict whether that article is misinformative or not. We use the scores of the Decision Tree, Logistic Regression, Random Forest Classifier, and SVM to test our models’ accuracies. After our models make a prediction on a random genre article, we want to examine differences of misinformation across different genres of news. </p>
<h2>What models are we using for prediction</h2>
<h3>Decision Tree </h3>
<p align="center"> <img src="assets/img/decision_tree_example.png"> </p>

<p>Decision Tree is a machine learning method that involves many leafs and branches to reach a classification.</p>


<h3>Logistic Regression</h3>
<p align="center"> <img src="assets/img/logistic_regression_example.png"> </p>

<p>Logisitic Regression is a machine learning method that results in a discrete (1,0) classification based on variables inputted.</p>


<h3>Random Forest Classifier</h3>
<p align="center"> <img src="assets/img/random_forest_classifier.png"> </p>

<p>Random Forest Classifier is a machine learning method that runs multiple decisions trees and uses the classification the majority choses.</p>


<h3>Support Vector Machine (SVM)</h3>
<p align="center"> <img src="assets/img/svm_example.png"> </p>

<p>Support Vector Machine is a machine learning method used to find the best hyperplane that separates the data into two distinct classes.</p>


<h3>Data Analysis</h3>
<p>Since our goal was to see if there were themes to the misinformation of each topic. We looked at what words would be the most important in deciding between misinformation. For consistency, we used logisitic regression as our base model for determining these clouds.</p>

<p align="center"> <img src="assets/img/science_logisitic_cloud (1).png"> </p>

<p>The image above is the word cloud of most important words for informative science articles. The most interesting words of informative science's word cloud are Lexus, chip, honey, and Ukraine. This result is interesting because it shows that informative science articles mainly focus on subject of the article.</p>

<p align="center"> <img src="assets/img/science_logisitic_cloud_false.png"> </p>

<p>The image above is the word cloud of most important words for misinformative science articles. The most interesting words that are visible by this word cloud are part, time, well, and more. These words are 
interesting because they are all descriptive words compared to the focus on the subject of the informative science articles.</p>

<p align="center"> <img src="assets/img/economics_logisitic_cloud (1).png"> </p>

<p>The image above is the word cloud of most important words for informative economic articles. The most interesting words of informative economy's word cloud are been, when, and without. This result is different compared to informative science articles where its main focus were the subject of the article. Economic's informative article focuses more on occasions.</p>

<p align="center"> <img src="assets/img/economics_logisitic_cloud_false.png"> </p>

<p>The image above is the word cloud of most important words for misinformative economic articles. The most interesting words of misinformative economy's word cloud are also, from, elected, and on. This result focuses a lot more on actions rather than the subject of the article.</p>

<p align="center"> <img src="assets/img/politics_logisitic_cloud.png"> </p>

<p>The image above is the word cloud of most important words for informative political articles. The most interesting words of informative politics's word cloud are Florida, the, Maher, Romney, and King. This result is a similar case to informative science article's results. There is more focus onto the subject of the article.</p>

<p align="center"> <img src="assets/img/politics_logisitic_cloud_false.png"> </p>

<p>The image above is the word cloud of most important words for misinformative political articles. The most interesting words of misinformative politics's word cloud are has, was, more, told, and did. This result is similar to misinformative economic article's results. There is more focus on to the action rather than the subject of the article.</p>

<p align="center"> <img src="assets/img/general_logisitic_cloud.png"> </p>

<p>The image above is the word cloud of most important words for informative articles with the topics science, economy, and politics all combined. The most interesting words for this word cloud are Covid, the, Romney, billion, playing, and wealth. The result is interesting since there are mixture of focus onto subject and description of the subject.</p>

<p align="center"> <img src="assets/img/general_logisitic_cloud_false.png"> </p>

<p>The image above is the word cloud of most important words for misinformative articles with the topics science, economy, and politics all combined. The most interesting words for this word cloud are high, most, nearly, several, and more. This result is interesting because these descriptive words are mostly used to describe more of something. Based on the nature of misinformation, it could be hypothesize that misinformative articles use these kinds of descriptive words to exaggerate the subject of its article.</p>

<h2>Results and Conclusions</h2>
<h3>Accuracy Percision and Recall</h3>
<p>As is consistent with the other projects that look at this issue, we ended up with somewhat lower accuracies. The results below are our top performers for each topic.</p>
<h4>General</h4>
<p align="center"> <img src="assets/img/general_acc.PNG"> </p>
 
<h4>Science</h4>
<p align="center"> <img src="assets/img/science_accPNG.PNG"> </p>
 
<h4>Economics</h4>
<p align="center"> <img src="assets/img/economics_acc.PNG"> </p>
 
<h4>Politics</h4>
<p align="center"> <img src="assets/img/politics_acc.PNG"> </p>

<p>We certainly had variances in success, but our best performing model was the science decision tree, with an accuracy of about 87%.</p>

<h3>Commonalities</h3>
<p>The next part of our project was finding if these models overlapped in some way, so we looked at how much their list of important words intersected with each other. For example, we found that the highest intersection was the intersection between General and Politics decision trees, with a similarity of 53.6%. An example of a limited intersection was the Science SVM model with the Politics Decision-Tree model with a similarity of 2.4%. While there are some limitation to this method, such as magnitude, we feel it shows important ways that these articles overlap in subject matter and in informativeness.</p>
