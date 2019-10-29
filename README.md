<h1><center>DS 5500 Assignment 1</center></h1>

<h2><center>Problem 1</center></h2>
Project group: https://piazza.com/class/k05u5i0wc3w540?cid=242

<h2><center>Problem 2</center></h2>

I have chosen the following visualization to answer this question: 
https://github.com/tonytontian/DS5500/tree/master/hw1

The visualization clearly explains the distribution of income (GDP / capita) across countries and continents over time. It looks very similar to my visulazation except that 5 static plots were used to show the distribution across 5 different years, where as I used an interactive slider to show the distribtion for each year. An interactive plot would have been more appropriate for this question, since it allows us to include more information about GDP per capita with respect to time.

The plots look easy to interpret and effectively visualizes what is asked but including an interactive plot could surely make it better.

<h2><center>Problem 3</center></h2>

I have chosen the following visualization to answer this question: 
https://github.com/noahdemoes/DS5500_Homework1

The visualization explains relationship between income (GDP / capita), life expectancy, and child mortality over time. The plots look very different from the approach I have used. One of the major difference is having 3 separate static plots corresponding to visualize income, life expectancy, and child mortality over time. Instead, I have used a single plot to visualize all three variables with time as a slider.

The visulaztion is easy to interpret and is effective in visualizing what is asked in the question. But, having 3 different plots could make it hard for cross relational analysis of the 3 variables over time.

<h2><center>Problem 4</center></h2>

I have used simple linear regression model to quantify the relationship betweem income (GDP per capita) and life expectancy over time. GDP was used as the predictor variable and Life expectancy as the target variable in all the models analysed.

Model 1: GDP vs Life Expectancy

<img src="https://github.com/ItsmeKumar/DS5500-HW2/blob/master/plots/gdp_le.png" width="675" height="400">

Model 2: log(GDP) vs Life Expectancy

<img src="https://github.com/ItsmeKumar/DS5500-HW2/blob/master/plots/loggdp_le.png" width="675" height="400">

Model 3: GDP vs log(Life Expectancy)

<img src="https://github.com/ItsmeKumar/DS5500-HW2/blob/master/plots/gdp_logle.png" width="675" height="400">

Model 3 has least RMSE of all, but considering RMSE would lead to bias, since models with log function applied to the target variable will always have lower RMSE. Model 2 is the best fit as it has highest variance explained and least p-value compared to other models.

The plots correspoding to every model show a clear positive correlation between GDP and Life Expectancy, which means the Life Expectancy tends to go up when GDP increases.


<h2><center>Problem 5</center></h2>

Linear regression was selected to quantify the relationship betweem income (GDP per capita) and child mortality over time. GDP was used as the predictor variable and Child Mortality as the target variable in all the models analysed.


Model 1: GDP vs Child Mortality

<img src="https://github.com/ItsmeKumar/DS5500-HW2/blob/master/plots/gdp_cm.png" width="675" height="400">

Model 2: log(GDP) vs Child Mortality

<img src="https://github.com/ItsmeKumar/DS5500-HW2/blob/master/plots/loggdp_cm.png" width="675" height="400">

Model 3: GDP vs log(Child Mortality)

<img src="https://github.com/ItsmeKumar/DS5500-HW2/blob/master/plots/gdp_logcm.png" width="675" height="400">

Model 3 has highest explained variance and least p-value of all the models. And plots of every model show a negative correlation between GDP and Child Mortality, which implies that Child Mortality will decrease as GDP increases.

Autocorrelation: We are assuming that there is no autocorrelation for our models in Problem 4 and 5. Autocorrelation of the errors violates the ordinary least squares assumption that the error terms are uncorrelated, meaning that the Gauss Markov theorem does not apply, and that OLS estimators are no longer the Best Linear Unbiased Estimators 
