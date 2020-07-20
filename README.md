# Starbucks-Capstone-Challenge

### Installations:
- import pandas as pd
- import numpy as np
- import math
- import json
- from datetime import datetime
- from time import time
- import matplotlib.pyplot as plt
- import seaborn as sns
- import warnings
- from sklearn.naive_bayes import GaussianNB
- from sklearn.ensemble import AdaBoostClassifier
- from sklearn.metrics import accuracy_score,f1_score
- from sklearn.model_selection import train_test_split,GridSearchCV
- from sklearn.naive_bayes import GaussianNB
- from sklearn.neighbors import KNeighborsClassifier
- from sklearn.svm import SVC


### Project Overview
- The program used to create the data simulates how people make purchasing decisions and how those decisions are influenced by promotional offers.
- Each person in the simulation has some hidden traits that influence their purchasing patterns and are associated with their observable traits. People produce various events, including receiving offers, opening offers, and making purchases.
- As a simplification, there are no explicit products to track. Only the amounts of each transaction or offer are recorded.
- There are three types of offers that can be sent: buy-one-get-one (BOGO), discount, and informational. In a BOGO offer, a user needs to spend a certain amount to get a reward equal to that threshold amount. In a discount, a user gains a reward equal to a fraction of the amount spent. In an informational offer, there is no reward, but neither is there a requisite amount that the user is expected to spend. Offers can be delivered via multiple channels.
- The basic task is to use the data to identify which groups of people are most responsive to each type of offer, and how best to present each type of offer.

### Problem Statement
- How could build a machine learning model that predicts how much someone will spend based on demographics and offer type. 
- How could build a model that predicts whether or not someone will respond to an offer? Or, you don’t need to build a machine learning model at all. You could develop a set of heuristics that determine what offer you should send to each customer (i.e., 75 percent of women customers who were 35 years old responded to offer A vs 40 percent from the same demographic to offer B, so send offer A).

### File Descriptions
### profile.json
- gender: (categorical) M, F, O, or null
- age: (numeric) missing value encoded as 118
- id: (string/hash)
- became_member_on: (date) format YYYYMMDD
- income: (numeric)

### portfolio.json
- reward: (numeric) money awarded for the amount spent
- channels: (list) web, email, mobile, social
- difficulty: (numeric) money required to be spent to receive reward
- duration: (numeric) time for offer to be open, in days
- offer_type: (string) bogo, discount, informational
- id: (string/hash)

### transcript.json
- person: (string/hash)
- event: (string) offer received, offer viewed, transaction, offer completed
- value: (dictionary) different values depending on event type
- offer id: (string/hash) not associated with any "transaction"
- amount: (numeric) money spent in "transaction"
- reward: (numeric) money gained from "offer completed"
- time: (numeric) hours after start of test

### Results
My blog post https://medium.com/@puchalapalli.gowthami/starbucks-capstone-challenge-2c20d1d54695

### Licensing, Authors, Acknowledgements, etc
Data for coding project was provided by Udacity.




