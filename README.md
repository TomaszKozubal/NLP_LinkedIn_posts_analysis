# Predicting LinkedIn Post Reach Using Regression Neural Network

## Project Overview
This project uses data from a SaaS platform for Employer Branding on LinkedIn. The dataset consists of CSV files, each representing all posts made by a single client (i.e., an instance of the platform). The goal is to predict the potential reach of a LinkedIn post based on variables that are under user control.

A regression neural network model was trained to estimate post reach using the following features:

✍️ Post copy (text)

👥 Current network size

⏰ Post time

📄 Post type: ['LINK', 'NATIVE_GALLERY', 'VIDEO', 'NATIVE_FILE', 'TEXT', 'DOCUMENT']

## Methodology
1. Data Preprocessing

2. Posts with reach >3,000 were considered outliers and excluded to improve general accuracy.

3. Text was tokenized and then embedded

4. Categorical variables were hot-encoded 

## Model

A regression neural network was made using PyTorch.

Optimized to minimize RMSE (root mean square error).

Training Results

Full Dataset:

Mean Reach: ~1,100

RMSE: ~350

Filtered Dataset (Reach ≤ 3,000):

Mean Reach: ~610

RMSE: ~220

This filtering significantly improved proportional accuracy and reduced the influence of rare viral outliers.
