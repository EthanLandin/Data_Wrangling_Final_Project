# 3250-Final-Project
### Final project for Data wrangling class

The 2 main folders in this repository are "Data" and "Mid Program Saves"
 - Data contains the initial data for the analysis
 - Mid Program Saves contains all saves throughout the project (including final csv file)
 - Python code is in file Final_Project_New.ipynb
 - Final Report is in file "Final Report - ELandin.pdf"

# File Names and Descriptions
| File Name | Description |
| ------ | ------ |
| company_ipo.csv | [initial IPO data] from Kaggle.com |
| Final_Project_New.ipynb | Jupyter notebook file with project code in it |
| Final Report - ELandin.pdf | Final report over findings |
| IPO_Data_1.csv | First mid-code save |
| IPO_Data_2.csv | Second mid-code save |
| IPO_Data_3.csv | Third mid-code save |
| IPO_Data_4.csv | Fourth mid-code save |
| Project_Data_Final.csv | Final csv file |


[initial IPO data]: <https://www.kaggle.com/datasets/shivamb/company-ipos-2019-2021>

# Data Dictionary
| Field Name             | Data Type | Source                 | Description                                                                                 |
|-----------------------|----------|-------------------------|---------------------------------------------------------------------------------------------|
| IPO Date              | object   | Kaggle                  | The calendar date the company went public (Initial Public Offering).                          |
| Symbol                | object   | Kaggle                  | The stock ticker symbol representing the company.                                             |
| Company Name          | object   | Kaggle                  | Full legal name of the company that went public.                                               |
| IPO Price             | float64  | Kaggle                  | The price per share at the time of the IPO.                                                    |
| Current               | float64  | Kaggle                  | Stock price as of December 21, 2021.                                                           |
| Return                | float64  | Kaggle                  | Percent return from IPO Price as of December 21, 2021.                                         |
| Market Cap            | float64  | StockAnalysis.com        | Market capitalization in millions of dollars at the time of scraping.                          |
| Year                  | int64    | Kaggle                  | The calendar year in which the IPO occurred.                                                   |
| Industry              | object   | YFinance                | The industry classification for the company.                                                  |
| Price_1W              | float64  | YFinance/Selenium       | Stock price 1 week after the IPO date.                                                         |
| Price_1M              | float64  | YFinance/Selenium       | Stock price 1 month after the IPO date.                                                        |
| Price_6M              | float64  | YFinance/Selenium       | Stock price 6 months after the IPO date.                                                       |
| Price_1Y              | float64  | YFinance/Selenium       | Stock price 1 year after the IPO date.                                                         |
| Return_1W_pct         | float64  | Calculated              | Percent return from IPO Price to Price_1W.                                                     |
| Return_1M_pct         | float64  | Calculated              | Percent return from IPO Price to Price_1M.                                                     |
| Return_6M_pct         | float64  | Calculated              | Percent return from IPO Price to Price_6M.                                                     |
| Return_1Y_pct         | float64  | Calculated              | Percent return from IPO Price to Price_1Y.                                                     |
| Market Cap Size       | object   | Derived                 | Categorical variable: Small Cap (<300M), Mid Cap (300M–2B), Large Cap (>2B).                    |
| Success_Q2            | int64    | Derived                 | Binary indicator: 1 if Return_1Y_pct > 0, otherwise 0.                                          |

