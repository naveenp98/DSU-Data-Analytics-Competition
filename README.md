# Dakota State University National Data Analytics Competition

## Introduction
Credit card default prediction is a vital task in the realm of financial risk management, aiming to forecast the likelihood of a credit card holder defaulting on their payments. Default prediction models play a crucial role in enabling financial institutions to assess and mitigate potential risks associated with extending credit to customers.

## Problem Statement
Can we predict whether a customer defaults on their credit payment using unlabeled, imbalanced data?

## Executive Summary
The train and test data consisted of unlabeled data of customers' payment information that were masked. 
Since the datasets required a lot of preprocessing, a helper function was designed to encode, impute and transform the dataset.

The model used was a LightGBM ML model that was tuned appropriately to provide accurate predictions. 10-fold cross validation was used on train-test splits that were transformed using the helper function to generate 10 different AUC-ROC curves. 

A threshold of 0.5 was used to generate binary predictions which were then submitted. These predictions were accurate enough to bag 3rd place and win $1000.
