# Predicting Whether a Country is Developed Or Developing based on Different Factors

## Made by
Ned Liu, Shaohuan Xia, Philip Davey

## Data Source
https://www.kaggle.com/datasets/lashagoch/life-expectancy-who-updated

## Predictors
- Infant_deaths: Infant deaths per 1000 population
- Under_five_deaths: Deaths of children under five years old per 1000 population
- Adult_mortality: Deaths of adults per 1000 population
- Alcohol_consumption: Alcohol consumption that is recorded in liters of pure alcohol per capita with 15+ years old
- Hepatitis_B: % of coverage of Hepatitis B (HepB3) immunization among 1-year-olds.
- Measles: % of coverage of measles-containing vaccine first dose (MCV1) immunization among 1-year-olds
- BMI
- Polio: % of coverage of Polio (Pol3) immunization among 1-year-olds.
- Diphtheria: % of coverage of Diphtheria tetanus toxoid and pertussis (DTP3) immunization among 1-year-olds.
- Incidents_HIV: Incidents of HIV per 1000 population aged 15-49
- GDP_per_capita: GDP per capita in current USD
- Population_mln: Total population in millions
- Thinness_ten_nineteen_years: Prevalence of thinness among adolescents aged 10-19 years. BMI < -2 standard deviations below the median.
- Thinness_five_nine_years: Prevalence of thinness among children aged 5-9 years. BMI < -2 standard deviations below the median.
- Schooling: Average years that people aged 25+ spent in formal education
- Life_expectancy: Average life expectancy of both genders in different years from 2010 to 2015

For the country status, 1 represents a developed country and 0 represents a developing country.

## Data Cleaning
The dataset is already cleaned by the creator. All null or 0 values are filled in.

## Train Test Split
75% of the dataset is used for training while the other 25% is used to test the final logistic regression model.

## Model 1
<img src="https://github.com/lybned/STAT-429-Group-Project/blob/main/Group%20Project/Model%201.PNG" width="500">

### Model 1 VIF
![alt text](https://github.com/lybned/STAT-429-Group-Project/blob/main/Group%20Project/Model%201%20Vif.PNG)

### Model 1 Testing Results
![alt text](https://github.com/lybned/STAT-429-Group-Project/blob/main/Group%20Project/Model%201%20Result.PNG)


## Model 2 (Backward BIC from Model 1)
<img src="https://github.com/lybned/STAT-429-Group-Project/blob/main/Group%20Project/Model%202.PNG" width="500">

### Model 2 VIF
![alt text](https://github.com/lybned/STAT-429-Group-Project/blob/main/Group%20Project/Model%202%20Vif.PNG)

### Model 2 Testing Results
![alt text](https://github.com/lybned/STAT-429-Group-Project/blob/main/Group%20Project/Model%202%20Result.PNG)\


## Model 3 (Backward AIC from Model 1)
<img src="https://github.com/lybned/STAT-429-Group-Project/blob/main/Group%20Project/Model%203.PNG" width="500">

### Model 3 VIF
![alt text](https://github.com/lybned/STAT-429-Group-Project/blob/main/Group%20Project/Model%203%20Vif.PNG)

### Model 3 Testing Results
![alt text](https://github.com/lybned/STAT-429-Group-Project/blob/main/Group%20Project/Model%203%20Result.PNG)


## Model 4 (All Subset Selection from Model 1)
<img src="https://github.com/lybned/STAT-429-Group-Project/blob/main/Group%20Project/Model%204.PNG" width="500">

### Model 4 VIF
![alt text](https://github.com/lybned/STAT-429-Group-Project/blob/main/Group%20Project/Model%204%20Vif.PNG)

### Model 4 Testing Results
![alt text](https://github.com/lybned/STAT-429-Group-Project/blob/main/Group%20Project/Model%204%20Result.PNG)


## Final Model (Model 2)

We decided to pick model 2 as the final model because it does NOT have collinearity issues, and its performance on the testing dataset is very good. It is also the simplest model out of all the models we have.


## Anova Test with Model 1 and 2
![alt text](https://github.com/lybned/STAT-429-Group-Project/blob/main/Group%20Project/Anova%20m1%20m2.PNG)

## Marginal Plots of Model 2
![alt text](https://github.com/lybned/STAT-429-Group-Project/blob/main/Group%20Project/Model%202%20Marginal%20Plots.png)
