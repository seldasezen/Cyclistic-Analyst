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
