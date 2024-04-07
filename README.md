# Content
* Images
  * All visuals created during analysis
* Resources
  * data.csv
    * Original Kaggle Data
  * esg_complete.csv
    * Cleaned csv combining Kaggle Data with API data
* Final Data
  * Final Analysis and Conclusion
  * Figures 
* Slide Deck

# Overview
We are an investment firm and many of our younger, Millenial and Gen Z investors, have become increasingly interested is companies and their ESG score. We have recieved several enquiries from our clients all centered around one question. 

Can I use a company's ESG score to determine whether or not I should invest in a company?

We secured a dataset from Kaggle.com, containing 722 companies spread across 47 Sectors, this dataset contained ESG grading and scoring. (where was their data derived) (quick ref to where this is in our repo). This grading broke the companies into grading bins, AA, A, BBB, BB, B. 

We then used the AlphaVantage API to pull stock data for the companies in order to isolate 5 year price average and EPS data. We were able to clean and merge our API data into one dataset, (name of that dataset)

* What are the top scoring ESG companies, and what are the top scoring industries by average total ESG score?
* How do the comapnies in our initial dataset breakdown by ESG total grade?

### In order to answer our general question our analysis primarily focuses on the follwing questions:
* Based solely on ESG total score, is there a positive and meaningful correlation between 5 year annualized change in stock price?
* Based solely on ESG total score, is there a positive and meaningful correlation between earnings per share (EPS)


# Analysis and Conclusion
From our analysis we have concluded that it would not be wise for investors to solely use ESG score as their lone indicator when deciding on their investment choices. Investors can certainly take a companies ESG rating into account when selecting an investment but factors such as Dividend Payout Ratio, Overall Investment Need, Time Horizon of the investor, Risk factor of the investor, Volatility of the stock/sector, and the overall stock market evnivornment need to be addressed in tandom with ESG grade when detmining the viability of a stock for a particular investor. 

For more detailed technical Analysis please see the ESG.ipynb Jupyter Notebook.

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
