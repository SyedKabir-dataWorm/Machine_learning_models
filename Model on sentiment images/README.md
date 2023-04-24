

* The source of the data: 
	- https://drive.google.com/drive/folders/1eWap2APLRbQltktO4j1bZNWyshMVailT?usp=sharing


**Details of the tasks**

Introduction

“A picture is worth a thousand words'' is an English idiom that is becoming more accurate
every day. Thanks to social networks, images have become one of the most important
communication tools in the world. Every day, users share millions of images and videos; in
most of the cases, this content is expected to convey effective information. As a result,
sentiment analysis is recently witnessing an increasing number of applications to multimedia
resources, in addition to text-only resources.

In this assessment, a data set that contains over twelve thousand
sentiment-scored images is given. Contributors were shown a variety of pictures (everything from
portraits of celebrities to landscapes to stock photography) and asked to score the images
on typical positive/negative sentiment. The data set contains the actual images (stored and
shared in Google Drive), sentiment scores of highly positive, positive, neutral,
negative, and highly negative, and contributor agreement. 

The task is to develop classification models which can make predictions and return the corresponding classification
of the source image. There are many machine learning methods that can be used in the
classification task and use few of them.

There are three major steps, including:
<br>- generating features,</br>
<br>- developing a proper classifier, and</br> 
<br>- applying the classifier to the unseen data.</br> 
The feature extractor is shared by both training and prediction, which tells us that data used in training
and prediction should share the same feature space. The aim of this challenge is to develop
a classifier that can assign the sentiment polarity of a set of general and public images to
their corresponding labels as correctly as possible.

Dataset:
<br>- Data Sourece : Public</br>
<br>- Data type: Image</br>
<br>- Classes: 5</br>
<br>- Name of training data-set : trainset_students.csv</br>
<br>- Number of training images: 9437</br>
<br>- Name of testing data-set : testset_students.csv</br>
<br>- Number of testing images: 9437</br>

Detailed Description of the Data-set:

● trainset_students.csv contains training IDs , labels and labels confidence:

1) ID: the unique image identifier. 
2) Label: the image sentiment polarity score. The labels are highly positive,
positive, neutral, negative, and highly negative.
3) Label_confidence: The confidence of the image Label between 0 to 1 where 1
indicates 100% confidence over the Label. Please note that each image is
manually labelled by several human annotators and this column indicates
their agreement with the image sentiment polarity.

● testset_students.csv: only testing ids are available. It contains 3146 images.

Data Preparation & Feature Extraction

Selecting relevant features and deciding how to encode them for a classification algorithm is
crucial for learning a good model. Raw images cannot be used directly as an input to
classification algorithms. It must be pre-processed and transformed into a set of features
represented in a numerical form.

Here are some useful resources that can give you some idea about feature extraction from images:

● https://towardsdatascience.com/image-feature-extraction-traditional-and-dee
p-learning-techniques-ccc059195d04
● https://kapernikov.com/tutorial-image-classification-with-scikit-learn/
● https://www.analyticsvidhya.com/blog/2019/08/3-techniques-extract-feature
s-from-image-data-machine-learning-python/
● https://freecontent.manning.com/the-computer-vision-pipeline-part-4-featureextraction/
● https://analyticsindiamag.com/image-feature-extraction-using-scikit-image-ahands-on-guide/
● https://tensorflow.rstudio.com/tutorials/beginners/basic-ml/tutorial_basic_cl
assification/
● https://analyticsindiamag.com/hands-on-guide-to-image-classification-using-r
/
● https://rpubs.com/spalladino14/653239

Classifier

The task is to develop a classifier that can give you the most accurate prediction in the
image sentiment polarity classification task. The algorithms that you can use are not limited
to the algorithms covered in the lectures/tutorials but the covered algorithms are enough to
achieve the performance thresholds in the marking rubric. The goal at this stage is to find the
most accurate classifier. In order to find the most accurate classifier, you should
empirically compare at least 3 different types of classification methods.Please note that an algorithm with
different input features will only count as one type of classifier. For example, logistic
regression will be counted as one type of classifier, no matter what features you used.

Evaluation

The evaluation method used in testing is the accuracy score, which is defined as the
proportion of correct predictions among all of the predictions.

𝑎𝑐𝑐𝑢𝑟𝑎𝑐𝑦 = 𝑛𝑢𝑚𝑏𝑒𝑟 𝑜𝑓 𝑐𝑜𝑟𝑟𝑒𝑐𝑡 𝑝𝑟𝑒𝑑𝑖𝑐𝑡𝑖𝑜𝑛𝑠 / 𝑛𝑢𝑚𝑏𝑒𝑟 𝑜𝑓 𝑎𝑙𝑙 𝑝𝑟𝑒𝑑𝑖𝑐𝑡𝑖𝑜𝑛s

Report

plagiarism check.

A pdf report, “report.pdf” is to be created. This pdf contains more detailed analysis of the
work. This file should show how you finished the task. Ideally you should show what
sort of algorithms you have considered, what kind of information you have used, and
the reason for your choice of the corresponding algorithm to achieve the results you
submitted on Kaggle. Comparison for different algorithms should be included in
this pdf report. Detailed analysis of the results are encouraged to display.The report includes:

a. The discussion of how the data preprocessing/features selection has been
done.

b. The development of the submitted classifier: To choose an optimal classifier
for a task, we often carry out empirical comparisons of multiple candidate
models with different feature sets. In your report, you should include a
comprehensive analysis of how the comparisons are done. For example, the
report can include (but not limited to)

i. A description of the classifier(s) considered in your comparison.
ii. The detailed experimental settings, which could include, for example,
the discussion of how the cross-validation is set up, how the
parameters for the model considered (if applicable) are chosen.
iii. Classification accuracy with comprehensive discussion.
iv. The justification of the final model submitted.

