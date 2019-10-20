## phishing-detection-challenge-in-url

As per wikipedia phishing is defined as the fraudulent attempt to obtain sensitive information such as usernames, passwords and credit card details, often for malicious reasons, by disguising as a trustworthy entity in an electronic communication.

### Problem definition -

This project is to apply machine learning to detect whether a website address is a phishing site or a genuine site. Training data consists of website address with information like domain registration, last update and expiry information. 

A function test_prep() is provided in the program that prepares the engineered features of training dataset for the test dataset. This function would be highly helpful to prepare unknown dataset before it can be used for prediction. 

The dataset provided should be divided in three parts naming train, validation, test dataset. train dataset woulde be used to train, validation dataset for the model validation and test dataset to predict. 

The model gives an accuracy of 94% on a chosen random test dataset.

The crux of the probelm is the preparation of certain advanced features that led to a high accuracy score without over-fitting. They are -

    •	URL length (Phising sites have higher length)  
    •	Total number of sub-domains in the URL (High for phising sites; inpersonating genuine sites in sub-domains makes it long)  
    •	Lower values of url last update age, expiry age for phising sites (Phising sites are purposed to perform the damage in short time) 
    •	Presence of high number of digits and certain special characters in phising sites.
  

