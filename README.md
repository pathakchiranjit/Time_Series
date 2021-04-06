### **The time-series project based on AQI data in Indian cities**


# Own Article link:
https://www.linkedin.com/posts/chiranjit-pathak-2261892a_timeseries-activity-6770680127278850049-gcMy


<img src="https://github.com/pathakchiranjit/Time_Series/blob/main/Pics/aqi5.gif?raw=true" align='left'><br/>

### An air quality index is used by government agencies to communicate to the public how polluted the air currently is or how polluted it is forecast to become. Public health risks increase as the AQI rises. Different countries have their own air quality indices, corresponding to different national air quality standards.

<img src="https://github.com/pathakchiranjit/Time_Series/blob/main/Pics/aqi3.gif?raw=true" align='left'><br/>

## Table of Contents

1. [Problem Statement](#section1)<br>
2. [Tools: Importing Packages](#section2)<br>
3. [Collecting & Loading Data](#section3)<br>
  - 3.1 [Importing Data sets & Description](#section301)<br>
  - 3.2 [Data Preparation](#section302)<br>
4. [Data Preprocessing](#section4)<br>
  - 4.1 [Data Preprocessing](#section401)<br>
5. [Exploratory Data Analysis](#section5)<br>
  - 5.1 [City wise AQI data analysis](#section501)<br>
  - 5.2 [AQI data analysis before and after COVID-19](#section502)<br>
  - 5.3 [AQI distribution for Delhi](#section503)<br>
6. [Time Series analysis and forecasting on AQI for delhi](#section6)
  - 6.1 [Trend,Seasonality study:](#section601)
  - 6.2 [Decomposition of time series:](#section602)
  - 6.3 [Stationarity check for source data:](#section603)
  - 6.4 [Base model using differencing methods:](#section604)
  - 6.5 [Model using SARIMAX methods:](#section605)
  - 6.6 [Prediction on validation set:](#section606)
  - 6.7 [Forecasting for next 100 days:](#section607)
  - 6.8 [Analysis of the forecasted data vs actual data (recorded separately):](#section608)
  - 6.9 [Modeling with ARIMA algorithm:](#section609)
	  - 6.9.1 [Auto Regressive Model:](#section6091)
	  - 6.9.2 [Moving Average Model:](#section6092)
	  - 6.9.3 [Auto Regressive Integrated Moving Average Model:](#section6093)
7. [Conclusion](#section7)

## Context:
Air is what keeps humans alive. Monitoring it and understanding its quality is of immense importance to our well-being.

<img src="https://github.com/pathakchiranjit/Time_Series/blob/main/Pics/aqi4.jpg?raw=true" align='left'><br/>

## Content:
The dataset contains air quality data and AQI (Air Quality Index) at hourly and daily level of various stations across multiple cities in India.

## AQI:
A tutorial of how AQI is calculated is available here: https://www.kaggle.com/rohanrao/calculating-aqi-air-quality-index

<img src="https://github.com/pathakchiranjit/Time_Series/blob/main/Pics/aqi2.png?raw=true" align='left'><br/>


## Cities from which measurement data taken:
Ahmedabad, Aizawl, Amaravati, Amritsar, Bengaluru, Bhopal, Brajrajnagar, Chandigarh, Chennai, Coimbatore, Delhi, Ernakulam, Gurugram, Guwahati, Hyderabad, Jaipur, Jorapokhar, Kochi, Kolkata, Lucknow, Mumbai, Patna, Shillong, Talcher, Thiruvananthapuram, Visakhapatnam

## Acknowledgements:
The data has been made publicly available by the Central Pollution Control Board: https://cpcb.nic.in/ which is the official portal of Government of India. They also have a real-time monitoring app: https://app.cpcbccr.com/AQI_India/

