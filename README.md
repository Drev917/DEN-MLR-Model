# DEN-MLR-Model

### Problem Statement: 
#### Assess patterns and correlation in non-airline revenue factors collected at DEN (Denver International Airport). Using data accrued from January 2012 - June 2017, create a method for forecasting non-airline revenues. Use it to produce forecasts for the months of March through June of 2017, and compare with the real observations to check your model performance. 

![ScreenShot](https://github.com/Drev917/DEN-MLR-Model/blob/main/NonAirline%20Slides/NA%201.JPG)



#### First we can look at our goals:
*On top of predicting total non-airline revenue as a comprehensive response variable, we looked at each of the dependent variables independently.

![ScreenShot](https://github.com/Drev917/DEN-MLR-Model/blob/main/NonAirline%20Slides/NA%202.JPG)

#### We then looked at the data as a whole to gain an idea of the different variables and observation values:

![ScreenShot](https://github.com/Drev917/DEN-MLR-Model/blob/main/NonAirline%20Slides/NA%203.JPG)

#### We used the following libraries to perform the EDA: 
- dplyr
- data.table
- tidyr
- janitor
- reshape2
- stats
- ggplot2

![ScreenShot](https://github.com/Drev917/DEN-MLR-Model/blob/main/NonAirline%20Slides/NA%204.JPG)

#### We also looked at seasonality between non-airline revenue and months/years as a timeseries

![ScreenShot](https://github.com/Drev917/DEN-MLR-Model/blob/main/NonAirline%20Slides/NA%205.JPG)

#### For our comprehensive non-airline revenue response variable: `TotalRev` we chose the following predictor variables as statistically significant and influential towards our regression model:

- `Month`
- `Destination`
- `Cannabis?`
- `UMCSENTLag3`

#### Adjusted Coefficient of Determination: 85.6%

![ScreenShot](https://github.com/Drev917/DEN-MLR-Model/blob/main/NonAirline%20Slides/NA%206.JPG)

#### We noticed non-normality of errors when plotting the residuals and checking for multiple linear regression violations of assumptions.
#### By performing a log transformation on the response variable `TotalRev`, we were able to spread our residual plot and correct any violations.

![ScreenShot](https://github.com/Drev917/DEN-MLR-Model/blob/main/NonAirline%20Slides/NA%207.JPG)

#### Lastly, an analysis was run on each of the factors that comprised the response variable in turn looking at residual standard error and ABS of the difference between training and test sets.

![ScreenShot](https://github.com/Drev917/DEN-MLR-Model/blob/main/NonAirline%20Slides/NA%208.JPG)

### Thanks for reading
