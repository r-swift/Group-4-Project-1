# Table of Contents

#### ESG.ipynb
* Main project analysis

#### data_clean.ipynb
* AlphaVantage API call and data clean and merge
       
#### csv_files
* data.csv (original data set from kaggle.com)
* esg_complete.csv (cleaned dataset used in main project analysis
      
#### Images
* output folder containing visuals generated during analysis
    
#### Slide Deck

# Overview
We are an investment firm and many of our younger, Millenial and Gen Z investors, have become increasingly interested is companies and their ESG score. We have recieved several enquiries from our clients all centered around one question. 

### Can I use a company's ESG score to determine whether or not I should invest in a company?

We secured a dataset from Kaggle.com, containing 722 companies spread across 47 Sectors, this dataset contained ESG grading and scoring. This grading broke the companies into grading bins, AA, A, BBB, BB, B. The Kaggle csv derived it's data from ESG Compare. This csv is within our data.csv file above.

We then used the AlphaVantage API to pull stock data for the companies in order to isolate annualized 5 year change in stock price and earnings per share (EPS) data for as many of the companies in our initial dataset as possible. The data claning and merge work can be found in data_clean.ipynb. Once complete we were able to  export it to csv, esg_complete.csv within the csv folder above. 

### To begin our analysis we started with the following questions:
* What are the top scoring ESG companies, and what are the top scoring industries by average total ESG score?
* How do the comapnies in our initial dataset breakdown by ESG total grade?

### In order to answer our general question our analysis primarily focuses on the follwing questions:
* Based solely on ESG total score, is there a positive and meaningful correlation between 5 year annualized change in stock price?
* Based solely on ESG total score, is there a positive and meaningful correlation between earnings per share (EPS)


# Analysis and Conclusion
Using our clean and merged dataset we ran a regression on ESG Total Score versus both EPS and Annualized % Growth. The resulting correlation from both studies was rather weak with Annualized % Growth having a correlation of 0.13 and EPS having a correlation of 0.2. Though these scores show there is a slight positive correlation between a companies ESG Total Score, their Earnings per Share, and their Annualized % Growth the correlation is not strong enough for us to recommend using ESG Total Score as a sole stock indicator. For more detailed technical Analysis please see the ESG.ipynb Jupyter Notebook.

As a result we have concluded that it would not be wise for investors to solely use ESG score as their lone indicator when deciding on their investment choices. Investors can certainly take a companies ESG rating into account when selecting an investment but factors such as Dividend Payout Ratio, Overall Investment Need, Time Horizon of the investor, Risk factor of the investor, Volatility of the stock/sector, and the overall stock market evnivornment need to be addressed in tandom with ESG grade when detmining the viability of a stock for a particular investor. 

# Resources

## Data Resources:
* ESG Compare - via Kaggle csv
  * https://www.kaggle.com/datasets/alistairking/public-company-esg-ratings-dataset
* AlphaVantage API
  * https://www.alphavantage.co/documentation/

## Background ESG Sources
* ESG Ratings Methodology
  * https://app.esgenterprise.com/uploads/ESG-Enterprise-Risk-Ratings-MethodologyV3.pdf
* Harvard Business Review
  * https://hbr.org/2022/08/esg-investing-isnt-designed-to-save-the-planet?ab=at_art_art_1x4_s01
* Nasdaq.com
  * https://www.nasdaq.com/articles/how-millennials-and-gen-z-are-driving-growth-behind-esg
* Harvard Law School of Coporate Governance
  * https://corpgov.law.harvard.edu/2022/03/16/the-false-promise-of-esg/
