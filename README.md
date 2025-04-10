# About the Project
This project for Time Series Analysis at Rennes School of Business aims to forecast ATM cash demand using time series analysis techniques. We analyze historical transaction data containing withdrawal amounts, transaction dates, and operational indicators to build predictive models that can optimize cash management strategies for financial institutions.

Our approach combines traditional statistical methods (SARIMA model) with machine learning techniques (ANN model) to identify patterns in daily/weekly cash withdrawals; compare manual and automated time series modeling approaches; and provide actionable insights for ATM cash replenishment. The collaborative effort among our team of 5 university students leverages our combined expertise in time series analysis, programming, and financial analytics to address the key question: "How can we accurately forecast ATM cash demand to optimize operational efficiency?"

The team originally worked using **[Google Colab with an R Kernel](https://colab.research.google.com/drive/1H9RPuwoMz6UycelYOxTnKf2mEtVKSxhs#scrollTo=OEKnMRZ1Umsn)**. The platform was chosen for its collaborative features, which allowed team members to work simultaneously on the code, share insights in real-time, and leverage the cloud-based environment for computational tasks.      

However, as the project progressed, and current complications were found while using R in Google Colab, the need for a more structured and reproducible format became apparent. To address it, the final script was transitioned to an .Rmd (R Markdown) format. The decision was made to enhance the practicality and usability of the script.     

## Team Members
* **[Li Bei](www.linkedin.com/in/bei-li-8484a6337)**
* **[Jiahui Zhong](linkedin.com/in/jiahui-zhong-2a8924328)**
* **[Riven Wu](www.linkedin.com/in/睿雯-伍-127925328)**
* **[Xian Harding Anglés](https://github.com/r41ss4)**
* **[Zhiying LIU](linkedin.com/in/芷颖-刘-a07146329)**

## The Dataset
The dataset contains detailed ATM transaction records obtained from **[Exploratory_Data_Analysis-on-ATM_transaction-dataset by Maheen Amin](https://github.com/maheenamin9/atm-transaction-eda)**. It includes 10434 rows and 9 columns, as the column `atm_name` was drop for the analysis. Key columns include include:        
* `transaction_date`: Date of each transaction
* `No_Of_Withdrawals`: Number of withdrawals per transaction
* `total_amount_withdrawn`: Total cash withdrawn
* `weekday`: Day of the week
* `working_day`: Business day indicator (H=Holiday, W=Working day)


## Project Structure
```
rennes_ts/          
│           
├── data/         
│   └── atm_transactions.csv        
│                       
├── scripts/                     
│   └── ts_analysis.Rmd                
│       
├── Insights.md               
└── README.md          
```


## Methodology
1. **Data Preparation**: It involves aggregating raw transaction data into daily time series format while addressing missing values and outliers. Time series decomposition separates the data into trend, seasonal, and residual components.          

2. **Exploratory Time Series Analysis**: It is examining daily and weekly patterns through visualization and statistical tests. Stationarity is assessed using ADF and KPSS tests, while ACF/PACF plots identify potential model parameters.      

3. **Modeling Approaches**: It is the comparation of manually specified SARIMA models with automated auto.arima() selections. Moreover, it was included an Artificial Neural Networks model, which provide an alternative machine learning approach for capturing complex patterns.       

4. **Model Evaluation**: It employs standard metrics including MAE, RMSE and MAPE to assess forecast accuracy. Residual diagnostics and out-of-sample testing validate model robustness across different time periods.      

## Conclusions
Feel free to review our findings in the file **[Insights.md](https://github.com/r41ss4/rennes_ts/blob/main/Insights.md)**. For more information, there is a full report available by request to team members of the project. 

## Tools and Technologies
- **R** (forecast, tseries, dplyr, ggplot2, neuralnet)
- **Google Colab** for collaborative development
- **GitHub** for version control
- **Markdown** for documentation