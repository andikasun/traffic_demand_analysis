# Grab AI Challenge

Grab AI Challenge consists of 3 challenges, Computer Vision, Safety and Traffic Demand Management. In this repository, I aimed to solve the Traffic Demand Challenge.

## Dependency

The code is run on Conda and Jupyter Notebook environment. Dependency list:
numpy, pandas, sklearn, matplotlib, geohash, hdbscan


## Files List
The repository consist of 3 files: 

#### grab_train_toy.csv
A small set of training data extracted from the original demand data set to demonstrate how to run the function.

#### Grab_demand-EXPLORATORY.ipynb
This is where the initial exploratory is run. Feature extraction, testing for various Machine Learning algorithm is conducted here. This file will take significant amount of time to run, around 20-40 minutes for 5% of the data sample. 
Major running time is at hdbscan and GridSearchCV processes.
The datasample can be adjusted in EXPLORATORY_SAMPLE.

#### Grab_demand-WORKING_FILE.ipynb
The data prediction is done here using the best algorithm and hyper parameters acquired from exploratory process.
To run the algorithm and get the resulting prediction CSV, call 
```python
predictTestSet( TEST_SET_CSV, PREDICTION_OUTPUT_CSV )
```
