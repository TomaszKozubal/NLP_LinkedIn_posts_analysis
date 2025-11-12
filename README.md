# Predicting LinkedIn Post Reach Using Regression Neural Network

## Project Overview
This project analyzes LinkedIn posts from a SaaS platform used for Employer Branding activities to predict post reach based on various features. The model uses a regression neural network that takes into account post content, network size, posting time, and post type to estimate potential reach.

A regression neural network model was trained to estimate post reach using the following features:

1. Post copy (text)

2. Current network size

3. Post time

4. Post type: ['LINK', 'NATIVE_GALLERY', 'VIDEO', 'NATIVE_FILE', 'TEXT', 'DOCUMENT']

## Key Features

Data Processing: Cleans and prepares LinkedIn post data from multiple clients

Natural Language Processing: Uses BERT tokenization and embeddings for post content analysis

Neural Network Model: Implements a regression neural network to predict post reach

Data Visualization: Includes visualizations of network size and reach distributions

Feature Engineering: Incorporates one-hot encoding for post times and formats

## Methodology

1. Data Preprocessing

2. Posts with reach >3,000 were considered outliers and excluded to improve general accuracy.

3. Text was tokenized and then embedded

4. Categorical variables were hot-encoded

5. NN model using Pytorch

## Limitations and Considerations

Data Constraints:

1. Model trained on posts with reach ≤ 3,000

2. May underestimate potential for viral content

3. Primarily trained on English-language content

### Performance Notes:

1. Better at predicting reach for mid-range posts than extremes

2. Accuracy improves with more representative training data

### Deployment Considerations:

1. Requires significant memory for BERT processing

2. Inference time depends on GPU availability

3. Model doesn't account for post engagement metrics (likes, comments)

## How to Use

Clone the repository

Install required libraries (see Dependencies section)

Place data files in /kaggle/input/data-sets-for-this-project/

Run the Jupyter notebook

## Dependencies

Python 3.11.11

PyTorch

Transformers (for BERT)

Pandas

NumPy

Scikit-learn

Matplotlib

### Note: The actual data files are not included in this repository as they are proprietary client data from a SaaS platform.
