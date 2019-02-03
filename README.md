##INTRODUCTION:

The advent of the Internet has definitely brought a significant sense of ease into our lives, but this ease sometimes comes at a price. The frequency of cybercrimes is booming exponentially. One of these crimes includes phishing, a cybercrime where an individual is tricked into giving extremely sensitive information about themselves by a seemingly reputable company or organization. This practice is done to retrieve credit card information, usernames, passwords and so on. Phishing is essentially the theft of user data. Hence, detection of phishing websites has been receiving a lot of attention recently due to their impact on users’ security. The goal is to create a function that predicts whether a website is a phishing website or not, when given the URL by using an accurate supervised learning approach.


##APPROACH:

Many supervised learning based classification based models such as Decision trees, Random forest, KNN and Bayesian Model were compared with their accuracy as shown below. 
Random Forest-96.3076700434%
Decision Tree-95.5861070912%
KNN-91.9319826339%
Bayesian Classification-58.2489146165%
Multinomial Logistic Regression-92.1490593343 %

Since the random forest model gives the highest accuracy in terms of classification models, it will be considered for the detection of malicious URLs.


##PREDICTOR FUNCTION:

The goal was to create a function that determines whether a website is a phishing website or not. To do so, a new dataset was created which was a subset of the original dataset. It contains attributes whose values could be determined when given the URL of the website. Since Random Forest classification gave the highest accuracy, the new dataset was trained using this technique and the new, revised model was obtained. The accuracy was now 66%, but this was sufficient since our function only used seven attributes to predict the result, which was all the attributes which could determined with limited knowledge. A predictor function was written which determines the values of each of the attributes of the new and smaller dataset. It then predicts the ‘Result’ attribute which determines if it is a phishing website or not. 


##FILES:
*dataset.csv* contains the dataset which was obtained from Kaggle. 
*Code.ipynb* contains the entire python code including all the various models which were created, along with preprocessing. It also contains the predictor function. 