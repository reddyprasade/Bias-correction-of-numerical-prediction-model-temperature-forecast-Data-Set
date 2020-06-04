# Bias-correction-of-numerical-prediction-model-temperature-forecast-Data-Set


**Problem Stastement**: It contains fourteen numerical weather prediction (NWP)'s meteorological forecast data, two in-situ observations, and five geographical auxiliary variables over Seoul, South Korea in the summer.

This data is for the purpose of bias correction of next-day maximum and minimum air temperatures forecast of the LDAPS model operated by the Korea Meteorological Administration over Seoul, South Korea. This data consists of summer data from 2013 to 2017. The input data is largely composed of the LDAPS model's next-day forecast data, in-situ maximum and minimum temperatures of present-day, and geographic auxiliary variables. There are two outputs (i.e. next-day maximum and minimum air temperatures) in this data. Hindcast validation was conducted for the period from 2015 to 2017.

***


|Data Set Characteristics|Number of Instances|Area|Attribute Characteristics|Number of Attributes|Associated Tasks|Missing Values|
|---------|-------|-----|----|---|---|---|
|Multivariate|7750|Physical|Real|25|Regression|Yes|



***

#### Atttributes Information
1. station - used weather station number: 1 to 25
2. Date - Present day: yyyy-mm-dd ('2013-06-30' to '2017-08-30')
3. Present_Tmax - Maximum air temperature between 0 and 21 h on the present day (Â°C): 20 to 37.6
4. Present_Tmin - Minimum air temperature between 0 and 21 h on the present day (Â°C): 11.3 to 29.9
5. LDAPS_RHmin - LDAPS model forecast of next-day minimum relative humidity (%): 19.8 to 98.5
6. LDAPS_RHmax - LDAPS model forecast of next-day maximum relative humidity (%): 58.9 to 100
7. LDAPSTmaxlapse - LDAPS model forecast of next-day maximum air temperature applied lapse rate (Â°C): 17.6 to 38.5
8. LDAPSTminlapse - LDAPS model forecast of next-day minimum air temperature applied lapse rate (Â°C): 14.3 to 29.6
9. LDAPS_WS - LDAPS model forecast of next-day average wind speed (m/s): 2.9 to 21.9
10. LDAPS_LH - LDAPS model forecast of next-day average latent heat flux (W/m2): -13.6 to 213.4
11. LDAPS_CC1 - LDAPS model forecast of next-day 1st 6-hour split average cloud cover (0-5 h) (%): 0 to 0.97
12. LDAPS_CC2 - LDAPS model forecast of next-day 2nd 6-hour split average cloud cover (6-11 h) (%): 0 to 0.97
13. LDAPS_CC3 - LDAPS model forecast of next-day 3rd 6-hour split average cloud cover (12-17 h) (%): 0 to 0.98
14. LDAPS_CC4 - LDAPS model forecast of next-day 4th 6-hour split average cloud cover (18-23 h) (%): 0 to 0.97
15. LDAPS_PPT1 - LDAPS model forecast of next-day 1st 6-hour split average precipitation (0-5 h) (%): 0 to 23.7
16. LDAPS_PPT2 - LDAPS model forecast of next-day 2nd 6-hour split average precipitation (6-11 h) (%): 0 to 21.6
17. LDAPS_PPT3 - LDAPS model forecast of next-day 3rd 6-hour split average precipitation (12-17 h) (%): 0 to 15.8
18. LDAPS_PPT4 - LDAPS model forecast of next-day 4th 6-hour split average precipitation (18-23 h) (%): 0 to 16.7
19. lat - Latitude (Â°): 37.456 to 37.645
20. lon - Longitude (Â°): 126.826 to 127.135
21. DEM - Elevation (m): 12.4 to 212.3
22. Slope - Slope (Â°): 0.1 to 5.2
23. Solar radiation - Daily incoming solar radiation (wh/m2): 4329.5 to 5992.9
24. Next_Tmax - The next-day maximum air temperature (Â°C): 17.4 to 38.9
25. Next_Tmin - The next-day minimum air temperature (Â°C): 11.3 to 29.8

## Process

### Data Collection

# UCI Machine Learning Repository in CSV

The UCI Machine Learning Repository is a collection of databases, domain theories, and data generators that are used by the machine learning community for the empirical analysis of machine learning algorithms.[UCI Machine Learning](https://archive.ics.uci.edu/ml/index.php)

## Data Set Colletion For UCI

* `Step-1`: Goto this [link](https://archive.ics.uci.edu/ml/datasets.php)
* `Step-2`: Select the Data Sets![](https://lh3.googleusercontent.com/-Qprd_P1bNeE/XkkiUnProdI/AAAAAAAAm2E/YAecsJa4keUvUppwOqC0MXZYga1HJEsmgCK8BGAsYHg/s0/2020-02-16.png)

* `Step-3`: Copy the Data Url ![](https://lh3.googleusercontent.com/-_eSgbi1-jOg/XkkirtydthI/AAAAAAAAm2M/NG5Xupis8nw6-HuynC6-gE6NYfMfZKwzACK8BGAsYHg/s0/2020-02-16.png)
* `Step-4`: Copy the Attribute Information:![](https://lh3.googleusercontent.com/-w6v3O1d_Tww/XkkjJumf7sI/AAAAAAAAm2U/uZI6zSkuMo48TrMO2nbH8_f7wkIcgJFygCK8BGAsYHg/s0/2020-02-16.png)


## Usage

```Python
import numpy as np
import pandas as pd

URL = "https://archive.ics.uci.edu/ml/machine-learning-databases/00514/Bias_correction_ucl.csv"

Data = pd.read_csv(URL)
Data.head()
```

## Contributing
If any one Intrested work with Use Pull requests are welcome. For major changes, please open an issue first to discuss what you would like to change.

Please make sure to update tests as appropriate.

## License
[MIT](https://choosealicense.com/licenses/mit/)[Copyright (c) 2020 REDDY PRASAD]
