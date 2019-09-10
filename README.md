# Taxi-Demand-Prediction-New-York-City


# Business Problem/Problem Statement
For a given location in New York City, our goal is to predict the number of pickups in that given location. Some location require more taxis at a particular time than other locations owing to the presence schools, hospitals, offices etc. The prediction result can be transferred to the taxi drivers via Smartphone app, and they can subsequently move to the locations where predicted pickups are high.

# Objectives & Constraints
Objectives: Our objective is to predict the number of pickups as accurately as possible for each region in a 10min interval. We will break up the whole New York City into regions, that we will discuss later in the blog. Now, the 10min interval is chosen because in NYC one can commute 1 mile in approximately 10 minutes given the traffic is normal at that particular time.

# Constraints:

 # Latency:
Given a location and current time of a taxi driver, as a taxi driver, he/she excepts to get the predicted pickups in his/her region and  the adjoining regions in few seconds. Hence, there is a medium latency requirement.

 # Interpretability: 
As long as taxi driver gets good prediction result, he/she is not be much interested in the interpretability of the result. He/she is not  much interested in why he/she is getting this result. Hence, there is a no interpretability required.

# Relative Errors:
Mean Absolute Percentage Error will be the relative error we will consider. Let say the predicted pickups for a particular location are   100, but actual pickups are 102, the percentage error will be 2% and Absolute error is 2. The taxi driver will be more interested in the  percentage error than the absolute error. Let say in some region the predicted pickups are 250, and if taxi driver knows that the relative  error is 10% then he/she will consider the predicted result to be in the range of 225 to 275, which is considerable.

**Our goal is to reduce the percentage error is low as possible**


# Source of Data:
**Data can be downloaded from here:**
http://www.nyc.gov/html/tlc/html/about/trip_record_data.shtml. **Here, we have used Jan- 2015 and Jan- 2016 data**

# Getting Started:
Start by downloading the project and run "Taxi-Demand-Prediction-NYC.ipynb" file in ipython-notebook.

You need to have installed following softwares and libraries in your machine before running this project.

Python 3: https://www.python.org/downloads/
Anaconda: It will install ipython notebook and most of the libraries which are needed like sklearn, pandas, seaborn, matplotlib, numpy and scipy: https://www.anaconda.com/download/


# Libraries:
# dask: It is used to handle very large files.
i) pip3 install dask

# folium: It is used to plot maps using latitude and longitude.
i) pip3 install folium
ii) conda install -c conda-forge folium

# xgboost: It is used to make xgboost regression model.
i) pip3 install xgboost
ii) conda install -c conda-forge xgboost

# gpxpy: It is used while we calculate the straight line distance between two (latitude, longitude) pairs in miles.
i) pip install gpxpy

