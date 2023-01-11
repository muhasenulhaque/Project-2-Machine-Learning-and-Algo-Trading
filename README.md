# FX_Master
> FinTech Project 2


![](./Images/intro_readme_img.jpg)


# Group Members

Pauline Liu, Flora Zhao, Md Muhasenul Haque
    

# Instructions on How to Read Through the Work

**1.** Please begin with the jupyter notebook file titled `fx_master_final.ipynb` which contains the retrospective analysis which has been conducted using historical data.

**2.** The csv files for the data used in this project can be found in the folder `Resources`. 

**3.** The presentation may be found under the folder `Presentation`.

**4.** The images used in the README file can be found under the folder `Images`.

**5.** In addition, for the purpose of choosing the best set of data to include in the models, we have also created two other alternative code files which contain different set of data. The file `fx_master_cash_interest.ipynb` only used the cash rate and interest rate for Australia and the USA. The file `fx_master_cash_interest_unemployment_indices.ipynb` added unemployment rate of Australia and the USA to the final version of code (`fx_master_final.ipynb`). The final version of code used the cash rate and interest rate for Australia and the USA in conjunction with USD index and Australian commodity price index. Please feel free to review the alternative versions of code, which can be found under the folder `Comparison`.

# Development

This code is built in Jupyter notebook. The process must be pretty much same when executing from GitBash on WindowsPC. If you are using VSCode then the required extensions/modules can be installed from VSCode GUI. To ensure, a suitable environment is existing to execute this code, you will need to have python3 and pip3 installed already. The Python version used to write this code is 3.9.12, any verison older than version 3 might not work efficiently.

# Dependencies

Apart from python3 and pip3, you will need to have jupyterlab, conda, anaconda, pandas, numpy, os, tradermade, pathlib, datetime, sklearn, matplotlib, tensorflow, scikitplot, python-dotenv installed at the operating system level.

The code is heavily dependent on pandas, numpy, sklearn, tensorflow and matplotlib modules.

Following modules must be already installed before running the code and conda environment must be activated as well. To execute the code, Jupyter notebook must be used. 

Below commands are Windows compatible to install required modules/tools.

As mentioned above ensure python3 and pip3 are already installed - preferrable version 3

	Install Jupyterlab

		pip install jupyterlab

	Install conda..

		pip install conda or brew install conda

	Install matplotlib..

		pip install matplotlib

	Install anaconda3..

		pip install anaconda3
	
	Install python-dotenv module..

		python3 -m pip3 install python-dotenv

	Install tradermade SDK

		pip install tradermade

	Installing scikit-learn

		pip install -U scikit-learn

	Install TensorFlow

		pip install --upgrade tensorflow     

	Install scikitplot

		pip install scikit-plot

	Install DateTime

		pip install DateTime 

	Install pathlib

		pip install pathlib

# Execution steps

To successfully execute the code...

conda environment must be created and activated.

	conda create -n cenv python=3.9.12
	conda activate cenv

To execute the code from Windows - you will need Visual Studio Code installed as well to look at the code.

The file 'fx_master_final.ipynb' is the file to be opened from the 'Jupyter notebook' interface ONLY.

Clone the directory which contains all the .csv files and the .ipynb file to your system using the following commands

	git clone https://github.com/muhasenulhaque/Project-2-Machine-Learning-and-Algo-Trading.git 

Once the clone completes.. 

	Go to the directory "Project-2-Machine-Learning-and-Algo-Trading"

	cd Project-2-Machine-Learning-and-Algo-Trading

Execute 'Jupyter notebook' command

In the Jupyter notebook interface, open the file 'fx_master_final.ipynb'

Please note, as the daily AUDUSD close price was pull from the tradermade API with an environment file (.env) on the local machine. For the readers' convenience, the close price has been saved as a csv file and was read back to the code file. Please do not load the part where it says "SKIP LOADING THIS PART". Instead, keep going down and start loading the code below the line where it says "START LOADING FROM HERE".


# Introduction

An exchange rate is a rate at which one currency will be exchanged for another currency and affects trade and the movement of money between countries.

Exchange rates are impacted by both the domestic currency value and the foreign currency value.

The exchange rate between two currencies is commonly determined by the economic activity, market interest rates, gross domestic product, and unemployment rate in each of the countries. Commonly called market exchange rates, they are set in the global financial marketplace, where banks and other financial institutions trade currencies around the clock based on these factors. Changes in rates can occur hourly or daily with small changes or in large incremental shifts.

# Motivation

This project is movitated by analysing different factors that may influence the fx rates, and try to use machine learning models to predict the moving direction of the exchange rate.

# Goals

1. Research on different factors that may have greater influence on the fx rate fluctuation
2. Predict the moving direction of the future fx rate (Up or Down) using binary classification
3. Compare different models and try to find the better model for the prediction

# Methodology & Steps
1. Data Preparation: Deciding on the factors that may influence the fx rates and how to pull of the historic data for the code
2. Train & Test the data: using different split of training/test data set to fine tune the optimised accuracy of the model
3. Make predictions and draw the plots
4. Model Evaluation

# Data Preparation and Model Training
## Factors that matters
- Unemployment Rate
- Interest Rate
- Inflation Rate
- USD index
- Australian commodity price index

## Model Summary
- LOGISTIC REGRESSION
- ADABOOST
- NEURAL NETWORK


# Conclusions / Results

## AdaBoost Performance

xxxxxxxxxxxxxxxxxxxxxxxxxxxxx
## Logistic Regression Performance

xxxxxxxxxxxxxxxxxxxxxxxxxxxxx
## Neural Network Performance

xxxxxxxxxxxxxxxxxxxxxxxxxxxxx

## Difficulties Faced

xxxxxxxxxxxxxxx



## Conclusion

xxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxx



## API and New Library

## New Machine Learning Models Used
- AdaBoost
## New Libraries Used
- Scikitplot : to plot the confusion metrics

## New APIs Used
- tradermade: to get historical/real-time close price for AUD/USD


# References

* **1** [6 Factors That Influence Exchange Rates](https://www.investopedia.com/trading/factors-influence-exchange-rates/)

* **2** [What Indicators Are Used in Exchange Rate Forecasting?](https://www.investopedia.com/ask/answers/021715/what-economic-indicators-are-most-used-when-forecasting-exchange-rate.asp)

* **3** [3 Examples of How Unemployment Rates Impact Currency Prices](https://www.valutrades.com/en/blog/3-examples-of-how-unemployment-rates-impacts-currency-prices)

* **4** [Australian Bureau of Statistics Unemployment Data and Statistics](https://www.abs.gov.au/statistics/labour/employment-and-unemployment/labour-force-australia/nov-2022#unemployment)

* **5** [Exchange Rate Prediction: Machine Learning with 5 Regression Models](https://towardsdatascience.com/exchange-rate-prediction-machine-learning-with-5-regression-models-d7a3192531d)

* **6** [Monthly Consumer Price Index Indicator](https://www.abs.gov.au/statistics/economy/price-indexes-and-inflation/monthly-consumer-price-index-indicator/latest-release)

* **7** [Federal Funds Rate - 62 Year Historical Chart](https://www.macrotrends.net/2015/fed-funds-rate-historical-chart)

* **8** [Consumer Price Index, Australia](https://www.abs.gov.au/statistics/economy/price-indexes-and-inflation/consumer-price-index-australia/latest-release)

* **9** [US Bureau of Labor Statistics Data CPI](https://data.bls.gov/timeseries/CUUR0000SA0&amp;amp;amp;output_view=pct_1mth)

* **10** [Ticks Volumns](https://forums.babypips.com/t/oanda-trading-volume/84294)

* **11** [Forex Data API](https://tradermade.com/forex)

* **12** [Change monthly data to daily in pandas](https://stackoverflow.com/questions/66759539/change-monthly-data-to-daily-in-pandas)

* **13** [Tutorial on Pandas Data-Reader](https://thecleverprogrammer.com/2021/03/22/pandas-datareader-using-python-tutorial/)

* **14** [Multiple Linear Regression With scikit-learn - GeeksforGeeks](https://www.geeksforgeeks.org/multiple-linear-regression-with-scikit-learn/)

* **15** [the difference between random_state = 0 & random_state = 1 | Data Science and Machine Learning](https://www.kaggle.com/discussions/getting-started/102258)

* **16** [Time Series Talk : ARIMA Model](https://www.simplilearn.com/top-python-libraries-for-data-science-article#8_pytorchhttps://www.youtube.com/watch?v=3UmyHed0iYE)

* **17** [statsmodels.tsa.arima.model.ARIMA](https://www.statsmodels.org/dev/generated/statsmodels.tsa.arima.model.ARIMA.html)

* **18** [AUD vs. US Dollar Index](https://en.macromicro.me/collections/345/mm-aud/18739/aud-dxy)

* **19** [Drivers of the Australian Dollar Exchange Rate](https://www.rba.gov.au/education/resources/explainers/drivers-of-the-aud-exchange-rate.html#:~:text=Australia%20has%20a%20floating%20exchange,in%20the%20foreign%20exchange%20market.)

* **20** [The Commodity Price and Exchange Rate Dynamics](https://www.scirp.org/journal/paperinformation.aspx?paperid=79731)

* **21** [Index of Commodity Prices](https://www.rba.gov.au/statistics/frequency/commodity-prices/2021/)

* **22** [How to Calculate Compound Investments Semi-Annually](https://budgeting.thenest.com/calculate-compound-investments-semiannually-26842.html)

* **23** [Historical inflation rates for United States of America](https://www.rateinflation.com/inflation-rate/usa-historical-inflation-rate/)

* **24** [Exchange Rate Prediction (Part 1): EDA & Data Visualisation](https://medium.com/analytics-vidhya/exchange-rate-prediction-part-1-276b6cd5338)

* **25** [Exchange Rate Prediction: Time Series Forecasting with ARIMA](https://medium.com/towards-data-science/exchange-rate-prediction-time-series-forecasting-with-arima-27260faafcdc)

* **26** [Top 10 Binary Classification Algorithms a Beginner’s Guid](https://towardsdatascience.com/top-10-binary-classification-algorithms-a-beginners-guide-feeacbd7a3e2)

* **27** [Classification: ROC Curve and AUC](https://developers.google.com/machine-learning/crash-course/classification/roc-and-auc)

* **28** [How to Plot a ROC Curve in Python (Step-by-Step)](https://www.statology.org/plot-roc-curve-python/)

---


*Jan 11th 2023*

---