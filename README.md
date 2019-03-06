# Unsupervised_Learning
Apply Unsupervised learning algorithms to two different datasets. I applied two clustering algorithms along with different dimensionality reduction algorithms and evaluated their performance in classifying the data correctly.

## Avocado Dataset
This dataset is comprised of information regarding avocado sales [Date, AveragePrice,
TotalVolume, SmHass, LgHass, ExLgHass, TotalBags, SmallBags, LargeBags, XLargeBags,
Type, Year, Region]. The data is particularly interesting because the avocado Type feature 
which indicates whether an avocado is standard or organic is relatively simple (binary) and 
easily separable as seen in previous assignments. Unsupervised learning
should be able to learn this feature without explicitly knowing the labels. Some features such as
volume are also separated into multiple highly related columns (small bags sold and large bags
sold) which indicate dimensionality reduction may perform well. 
Prior to implementing clustering and dimensionality reduction, the categorical features (region
sold and avocado type) were removed. I experimented with including them after one-hot
encoding and standardizing the data but clustering performed best, as expected, with strictly the
numerical data.

## Abalone Dataset
The Abalone dataset consists of physical measurements of abalone in Tasmania from the North
Coast and Islands of Bass Strait provided by the Marine Resources Division, Marine Research
Laboratories, and the Department of Primary Industry and Fisheries. The dataset contains the
following attributes: [Sex, Length, Diameter, Height, Whole weight, Shucked weight, Viscera
weight, Shell weight, Rings]
Unsupervised Learning methods will be using the information available about the abalone to
correctly predict its sex [‘m’, ‘f’, ‘infant’]. This dataset is interesting, in comparison to the avocado
problem, because it is easier to approach and interpret. There are only 8 predictor variables and
all but one of the predictor categories are continuous.

Language:
Python 2

IDE I used: 
Jupyter (Python)

OS I used: Mac OS

How to run code:
Make sure you have python 2.7 installed:
Python 2.7 :: Anaconda custom (x86_64)
iPython 6.1.0
Homebrew and pip

Necessary Libraries (can also be installed with conda):
Numpy  - pip install numpy
Pandas  -  pip install pandas
Seaborn  - pip install seaborn
Matplotlib  - brew install pkg-config, 
    - pip install matplotlib
Scikit-learn - pip install -U scikit-learn
SciPy - pip install scipy

Dataset Links:
https://archive.ics.uci.edu/ml/datasets/abalone
https://www.kaggle.com/neuromusic/avocado-prices/home

