# Data-preprocessing-characterstics
#Data preprocessing steps using pandas profiling
import pandas as pd
import numpy as np
import pandas_profiling

data=pd.read_csv('My_data.csv')

#Pandas Profiling
report = pandas_profiling.ProfileReport(data)
#covert profile report as html file
report.to_file("PandasProfiling.html")    #A HTML file will be created at the same location with the same of PandasProfiling.html
