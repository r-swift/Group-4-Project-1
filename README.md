# Content
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
We are an investment firm and many of our younger, Millenial and Gen Z investors, have become increasingly interested is companies and their ESG score. We have recieved several enquireies from our clients all centered around one question. 

Can I use a companies ESG rating to determine whether or not I should invest in a company?

We secured a ESG Grading Database from ESG Governance containing 722 companies spread across 47 Sectors. This grading broke the companies into grading bins, AA, A, BBB, BB, B. 

We then used the AlphaVantage API to pull stock data for the companies in order to isolate 5 year price average and EPS data.

* What are the top rated ESG companies?
* What are the average ESG ratings by Sector?
* What are the 5 year annualized averages and EPS scores for the avaliable bins AA, A, BBB, BB, B?
* Is there any correlation between the 5 year annualized averages and EPS data and ESG grade rating?

# Analysis and Conclusion
From our analysis we have concluded that it would not be wise for investors to solely use ESG grade as their lone indicator when deciding on their investment choices. Investors can certainly take a companies ESG rating into account when selecting an investment but factors such as Dividend Payout Ratio, Overall Investment Need, Time Horizon of the investor, Risk factor of the investor, Volatility of the stock/sector, and the overall stock market evnivornment need to be addressed in tandom with ESG grade when detmining the viability of a stock for a particular investor. 

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
