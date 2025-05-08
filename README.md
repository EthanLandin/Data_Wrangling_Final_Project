# 3250-Final-Project
### Final project for Data wrangling class

The 3 main folders in this repository are Data, Mid-Program Files, and Python Code
 - Data contains the initial data for the analysis, and 1 midround save after all scraping has been completed
 - Mid-Program files contains all csv saves throughout the python program
 - Python Code contains the .ipynb file with the actual project code in it

# File Names and Descriptions
| File Name | Description |
| ------ | ------ |
| company_ipo.csv | [initial IPO data] from Kaggle.com |
| stock_overview_scraped.csv | Initial data with new scraped columns included |
| ipo_data_2019_2021_cleaned.csv | First data save, after scraping updated prices |
| merged_ipo_cleaned1.csv | save after cleaning first columns of data |
| merged_ipo_cleaned2.csv | Save after scraping yfinance data for market cap |
| Final_ipo_data_cleaned.csv | Save after converting numbers into millions |
| Project_Part_2_Data.csv | Save after finishing part 2 of the project (current last save) |
| Project_Landin.ipynb | Python code for the project |


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

