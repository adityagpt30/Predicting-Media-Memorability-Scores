# Predicting-Media-Memorability-Scores

**TASK**

This is a media analytics task in which we have designed a machine learning algorithm that will be used to predict the memorability of short video clips. So, task is to design a machine learning algorithm which predicts these memorability scores from the videos. We asked test subjects to watch 10,000 seven-second video clips. They were subsequently asked about their recall of these videos. As a result we were able to annotate each video clip with a memorability score, based on how many people were able to successfully recollect the video. So we have the videos and target features - in this case the memorability score.

**ABSTRACT**

Memorability is defined as the state of being easy to remember or worth remembering. Nowadays with an increasing number of users in social media platforms, there are more than billions of videos that are viewed by us and when we see these videos it gets pivoted and focussed in our mind. Through these videos, our visual power is more grasping than the usual readings or listenings. Memorability thus rotates or oscillates in our mind to capture the attention of our brain clocks, as certain features have a sharp impact on our memorability. But now the question arises that how memorable these videos are to us? Or Are these videos worth remembering? Or Is there any feature which can predict the memorability. Therefore in this project, I have implemented various features with different algorithms in predicting the short-term and long-term memorability scores.

**INTRODUCTION**

In this project, we investigated the Media Memorability scores and further predicted the short-term and long-term scores based on the various features and using different algorithms. As part of the MediaEval Media Memorability challenge 2018, we were given short videos including different descriptive features to predict memorability such as InceptionV3, C3D, HMP, ColorHistogram, and so on. Initially,
I trained the models separately with all the given features but then later chose Captions, HMP, and Inception to predict the memorability as previous work has also shown us that using captions and HMP yields good results as compared to other features like ColorHistogram or C3D. Therein, I trained various models using different algorithms to predict the memorability score. The models are then evaluated using Spearman Correlational Coefficient.



**MODEL EXPLORATION**

I simply preferred linear regression algorithms for the prediction of memorability scores and ran different algorithms on different features like:

* For Captions, I used Random Forest Regression algorithm
and used Support Vector Regression algorithm.
* For HMP, I used Random Forest and Decision Tree
Regression algorithm.
* For Inception, I used Sequential Neural network algorithm.

*Based on the analysis it can be said that:*

* Captions yield better results than any other features available and whereas Inception being the worst.
* Short-term memorability scores were more accurate than the long-term memorability scores.
* If we increase the size of the test-set in the prediction the performance will go down and will become more sturdy.

**CONCLUSION**

The overall analysis shows us that captions provided us better short-term and long-term memorability scores when used as a feature with the Random Forest Regression Algorithm. Also, it can be said that short-term predictions are more precise than long-term predictions. Captions feature when used with Support Vector Regression Model also yields us good results but it was not better than the Random Forest Regression
algorithm.
