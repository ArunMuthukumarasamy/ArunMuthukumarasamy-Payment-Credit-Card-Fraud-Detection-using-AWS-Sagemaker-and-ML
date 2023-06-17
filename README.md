# ArunMuthukumarasamy-Payment-Credit-Card-Fraud-Detection-using-AWS-Sagemaker-and-ML
# Credit Card Fraud Detection 
# Introduction 
 IN this respository contains Credit card fraud detection algorithm using machine learning techniques in AWS Sage Maker.The increase of people using credit cards in theirdaily lives, credit cardcompanies should take special care in the security and safety of theircustomers. According to Credit card statistics 2021) the number of peopleusing credit cards around the world was 2.8 billion in 2019, in addition70%ofthose users own a single card at least. Reports of Credit card fraud in the US rose by 44.7% from 271,927 in 2019to 393,207 reports in 2020. There are two kinds of credit card fraud, the firstone is by having a credit card account opened under your name by an identitythief, reports of this fraudulent behavior increased 48% from 2019 to 2020. We used four different types of supervised and unsupervised algorithms to detect the fraud on credit cards payments, This project aims to focusmainly on machine learning algorithms.
 # Some familiar Algorithm are used in the project,
1. Logistic Regression.
2. Support Vector Machine(SVM).
3. Naive Bayes.
4. Random Forest.
# 1. Logistic Regression.
❖ Logistic Regression is basically effective for binary
classification problems.
# 2. Support Vector Machine(SVM).
❖ Support Vector Machine is effective for separating classes
in high-dimensional spaces.
# 3. Naive Bayes.
❖ Naive Bayes algorithm, which is used for classification
tasks, like text classification.
# 4. Random Forests.
❖ Random Forest algorithm is an ensemble of decision trees
for improved performance and robustness.
# Dataset 
The dataset was retrieved from an open-source website, Kaggle.com. It
contains data of transactions that were made in 2013 by credit card users in
Europe, in two days only. The dataset consists of 31 attributes, 284,808
rows. 28 attributes are numeric variables that due to confidentiality and
privacy of the customers have been transformed using PCA transformation,
the three remaining attributes are “Time” which contains the elapsed seconds
between the first and other transactions of each attribute, “Amount” is the
amount of each transaction, and the final attribute “Class” which contains
binary variables where “1” is a case of fraudulent transaction, and “0” is not
as case of fraudulent transaction.

➢ Gather credit card transaction data from relevant sources, such as
financial institutions or credit card processors. Ensure that the dataset
includes both legitimate and fraudulent transactions.

➢ Dataset has taken from kaggle datase : https://www.kaggle.com/datasets/mlg-ulb/creditcardfraud

# AWS Sage Maker setup
An Amazon SageMaker notebook instance is a fullymanaged machine learning (ML) Amazon Elastic Compute Cloud (AmazonEC2) compute instance that runs the Jupyter Notebook App. You use thenotebook instance to create and manage Jupyter notebooks for preprocessingdata and to train and deploy machine learning models.

![image](https://github.com/ArunMuthukumarasamy/ArunMuthukumarasamy-Payment-Credit-Card-Fraud-Detection-using-AWS-Sagemaker-and-ML/assets/123149917/b630f74b-7b9c-49cc-81d3-dc67b31c7d48)

1. Open the Amazon SageMaker console athttps://console.aws.amazon.com/sagemaker/.
2. Choose Notebook instances, and then choose Create notebookinstances.
3. On the Create notebook instance page, provide the followinginformation (if a field is not mentioned, leave the default values):
a. For Notebook instance name, type a name for your notebookinstance.
b. For Notebook Instance type, choose ml.t2.medium. This is theleast expensive instance type that notebook instances support,and it suffices for this exercise. Ifml.t2.medium instance type21isn't available in your current AWS Region, chooseml.t3.medium.
4. For Platform Identifier, choose a platform type to create the notebookinstance on. This platform type dictates the Operating System and theJupyterLab version that your notebook instance is created with. Forinformation about platform identifier type, see Amazon Linux 2 vsAmazon Linux notebook instances. For information about JupyterLabversions, see JupyterLab versioning.5. Choose Create notebook instance.In a few minutes, SageMaker launches an ML compute instance—inthis case, a notebook instanc—and attaches a 5 GB of Amazon EBSstorage volume to it. The notebook instance has a preconfiguredJupyter notebook server, SageMaker and AWS SDK libraries, and a set
of Anaconda libraries.For more information about creating a SageMaker notebook instance,see Create a Notebook Instance.
![Screenshot (23)](https://github.com/ArunMuthukumarasamy/ArunMuthukumarasamy-Payment-Credit-Card-Fraud-Detection-using-AWS-Sagemaker-and-ML/assets/123149917/43532024-acde-4399-a2dc-ed71d19181fc)

# Accuracy Comparison 
# Accuracy Comparison of Four Algorithms

1.Logistic Regression :            0.7526470588235294

2.Support Vector Machine(SVM)   :  0.6102941176470589

3.Naive Bayes                :     0.6617647058823529

4.Random Forest               :    0.8775158487705719

(According to our implementation of four supervised
learning, Random Forest has a better accuracy rate then the other
three algorithms.)

# Software Requirements

Server Side-> AWS Sage Maker

IDE Jupyter-> Notebook

Kernel Type-> Python 3

Instance Type-> Ml.M5.4xlarge 16 vcpu + 64gib

Operating System-> Windows 11

# Reference

➢Dataset has taken from kaggle data collection anonymized creditcard transactions labeled as fraudulent or genuine.

➢Dataset link : https://www.kaggle.com/datasets/mlg-ulb/creditcardfraud

➢Source Code has referred from- Hamza Nasir- from github

➢GitHub Link : Credit Card Fraud Detection using Machine Learning
inPython https://github.com/hamzanasirr/Credit-Card-Fraud-Detection-using-Machine-Learning

# Conclusion
In this paper we developed a novel method for fraud detection,
where customers are grouped based on their transactions and extract
behavioral patterns to develop a profile for every cardholder. Then different
classifiers are applied on three different groups; later rating scores are
generated for every type of classifier.. We finally observed that Logistic
regression and random forest are the algorithms that gave better results .

# Happy coding......;


