# Phishing Website Detection

## Introduction
Phishing is a type of cyber attack where attackers use social engineering techniques to trick victims into revealing their sensitive information, such as login credentials, credit card details, or other personal information.

## How Do We Detect It?
We employ Machine Learning techniques to detect whether a particular website is phishing or not. Specifically, we use Logistic Regression based on the semantic and network-based features of the URL. A manual threshold has been set to optimize the true positive rate.

The detailed implementation can be found in the [notebook on Kaggle](https://www.kaggle.com/code/tenzintsundue/phishing-website-detection).

## About the API
An API has been created to provide prediction results. The response is in JSON format and includes the following fields:

- **Result**: Indicates whether the website URL is phishing or not. [Possible Values: "Phishing", "Not Phishing"]
- **Result_binary**: Binary representation of the result. [Possible Values: -1 (phishing), 1 (legitimate)]
- **url**: Returns the URL that was tested.

## Steps to Use the API
To test if a website is phishing or not, use the following path:


