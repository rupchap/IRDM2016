# IRDM2016 - Information Retrieval and Data Mining 2016
## UCL group project - Time Series Forecasting

Team Members:
- Rupert Chaplin
- Artemis Dampa
- Megane Martinez

## Kaggle Global Energy Forecasting Competition 2012 - Load Forecasting

This project explores a number of different techniques to tackle a hierarchical load forecasting problem - a challenge which was released on Kaggle in 2012.

# Manual

## File Structure
Data - contains source datafiles, as provided for the Kaggle competition.

Data/Outputs - destination for any outputs generated by our code

Code - contains all scripts.

## Implementation
This project has been developed in Python 2.7.
Some elements require additional libraries/packages/hardware - as listed in requirements below.

## Code outline
## Models
### benchmark.py
This code runs a multiple regression to predict load values.  It replicates Tao Hong's 'vanilla benchmark' model.
http://repository.lib.ncsu.edu/ir/bitstream/1840.16/6457/1/etd.pdf

Requirements: Pandas, Numpy, SKLearn, matplotlib

main() can be run directly.

### nn.py
This code runs a neural network to predict load values.

Requirements: Pandas, Numpy, SKLearn, Keras (http://keras.io), Theano, compatible GPU hardware.

main() can be run directly.

### gradientboosting.py
This code runs a gradient boosting regression to predict load values.

Requirements: SKLearn, matplotlib.

main() can be run directly.

### arima.py
MEGANE

### arimaTemp.py
MEGANE

## Helper code
### processandmergedata.py
Contains data preprocessing steps.  This code includes helper functions, which are invoked by the modules below to provide data as required.
There is no need to run this script directly, although the main() function will create a set of csv files containing processed input data, which can be useful for debugging or exploratory data analysis in other packages.

### wrmse.py
This code contains a helper function to calculated Weighted Root Mean Square Error, which is the evaluation metric used for the Kaggle competition.
It called from other modules and not run directly.

### processTemp.py
MEGANE
