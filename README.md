# Predicting Whether a Country is Developed Or Developing based on Different Factors

## Data Source
https://www.kaggle.com/datasets/lashagoch/life-expectancy-who-updated

## Predictors
- Infant_deaths: Infant deaths per 1000 population
- Under_five_deaths: Deaths of children under five years old per 1000 population
- Adult_mortality: Deaths of adults per 1000 population
- Alcohol_consumption: Alcohol consumption that is recorded in liters of pure alcohol per capita with 15+ years old
- Hepatitis_B: % of coverage of Hepatitis B (HepB3) immunization among 1-year-olds.
- Measles: % of coverage of Measles containing vaccine first dose (MCV1) immunization among 1-year-olds
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

For the country status, 1 represents developed country and 0 represents developing country.

## Data Cleaning
The dataset is already cleaned by the creator. All null or 0 value are filled in.

## Train Test Split
75% of the dataset are used for training while the other 25% are used to test the final logistic regression model.

## Model 1
![alt text](https://github.com/lybned/STAT-429-Individual-Project/Group%20Project/blob/main/Pictures/Model%201.PNG)

### Model 1 VIF
![alt text](https://github.com/lybned/STAT-429-Individual-Project/Group%20Project/blob/main/Pictures/Model%201%20Vif.PNG)

### Testing Results
![alt text](https://github.com/lybned/STAT-429-Individual-Project/Group%20Project/blob/main/Pictures/Model%201%20Result.PNG)

