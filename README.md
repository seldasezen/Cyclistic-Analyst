# Cyclistic Bike Share Last 12 Months Analyst
The data is used in this case study to explore how different client types are using Cyclistic bikes. 
The dataset is public and available for download [here](https://divvy-tripdata.s3.amazonaws.com/index.html). The data has been made available by Motivate International Inc under this [license](https://www.divvybikes.com/data-license-agreement). 

## About the company
In 2016, Cyclistic launched a successful bike-share offering. Since then, the program has grown to a fleet of 5,824 bicycles that
are geotracked and locked into a network of 692 stations across Chicago. The bikes can be unlocked from one station and
returned to any other station in the system anytime.
Until now, Cyclistic’s marketing strategy relied on building general awareness and appealing to broad consumer segments.
One approach that helped make these things possible was the flexibility of its pricing plans: single-ride passes, full-day passes,
and annual memberships. Customers who purchase single-ride or full-day passes are referred to as casual riders. Customers
who purchase annual memberships are Cyclistic members.
Cyclistic’s finance analysts have concluded that annual members are much more profitable than casual riders. Although the
pricing flexibility helps Cyclistic attract more customers, Moreno believes that maximizing the number of annual members will
be key to future growth. Rather than creating a marketing campaign that targets all-new customers, Moreno believes there is a
very good chance to convert casual riders into members. She notes that casual riders are already aware of the Cyclistic
program and have chosen Cyclistic for their mobility needs.

## Dataset
For this case study, the available last 12 months of Cyclistic trip data which is between 2021/07-2022/06 are used for analysis.  

```python
# Imported Libraries
import numpy as np    
import csv                                
import os                                 
import glob                               
import pandas as pd                       
import warnings                           
import matplotlib.pyplot as plt           
import difflib                            
import re
import datetime as datetime
from datetime import timedelta
pd.options.mode.chained_assignment = None
import seaborn as sns
%matplotlib inline
```
Data was read by ```pd.read_csv ``` and concated by ```pd.concat``` function.

```python
# Imported Datasets
c2107= pd.read_csv("/Users/seldasezen/Desktop/cyclistic trip data_202107_202206/Trip data_cvs/202107-divvy-tripdata.csv")
c2108= pd.read_csv("/Users/seldasezen/Desktop/cyclistic trip data_202107_202206/Trip data_cvs/202108-divvy-tripdata.csv")
c2109= pd.read_csv("/Users/seldasezen/Desktop/cyclistic trip data_202107_202206/Trip data_cvs/202109-divvy-tripdata.csv")
c2110= pd.read_csv("/Users/seldasezen/Desktop/cyclistic trip data_202107_202206/Trip data_cvs/202110-divvy-tripdata.csv")
c2111= pd.read_csv("/Users/seldasezen/Desktop/cyclistic trip data_202107_202206/Trip data_cvs/202111-divvy-tripdata.csv")
c2112= pd.read_csv("/Users/seldasezen/Desktop/cyclistic trip data_202107_202206/Trip data_cvs/202112-divvy-tripdata.csv")
c2201= pd.read_csv("/Users/seldasezen/Desktop/cyclistic trip data_202107_202206/Trip data_cvs/202201-divvy-tripdata.csv")
c2202= pd.read_csv("/Users/seldasezen/Desktop/cyclistic trip data_202107_202206/Trip data_cvs/202202-divvy-tripdata.csv")
c2203= pd.read_csv("/Users/seldasezen/Desktop/cyclistic trip data_202107_202206/Trip data_cvs/202203-divvy-tripdata.csv")
c2204= pd.read_csv("/Users/seldasezen/Desktop/cyclistic trip data_202107_202206/Trip data_cvs/202204-divvy-tripdata.csv")
c2205= pd.read_csv("/Users/seldasezen/Desktop/cyclistic trip data_202107_202206/Trip data_cvs/202205-divvy-tripdata.csv")
c2206= pd.read_csv("/Users/seldasezen/Desktop/cyclistic trip data_202107_202206/Trip data_cvs/202206-divvy-tripdata.csv")

# Concacted Datasets
c12mnths=pd.concat([c2107, c2108, c2109, c2110, c2111, c2112, c2201, c2202, c2203, c2204, c2205, c2206])

```

