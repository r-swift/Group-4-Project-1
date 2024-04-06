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
* Is there any correlation between the 4 year annualized averages and EPS data and ESG grade rating?



# Analysis and Conclusion
We began our analysis by creating a clean csv file using combined data from the ESG csv and the API data calls from AlphaVantage. Once we had this csv we began to dive deeper into the data. 

We isolated and removed the outliers from the Annualized Growth and EPS data to reduce the amount of pull they would have one the overall dataset.

Our first step was to isolate the mean and median data for each Industry. This allowed us to see if there was a gross overweighting towards one industry as opposed to another. 

We then looked at the actual grading system that was avliable to us. This was an important piece of analysis for us as we were able to see that the BBB rating bucket accounted for 51% of the total population. This was important for us to realize moving forward as it could lead to larger sway within our studies. 

Next we plotted two linear regressions one for EPS data and one for Annualized Growth data from this we were able to determine that there was no real meaningfull correlation between EPS and Annualized Growth and ESG Grade. With low r-squared ratings idicating that there is a lower level of variation. However, between the two we can say that between Annualized Growth and EPS, EPS holds a higher correlation to ESG grade than Annualized Growth does. This makes sense as the EPS shows the actual earnings per share a company had as opposed to general stock price movement. However, the correlation score of 0.2 would indicate a weak relationship betwen the two variables. 

As a result, we have determined that is would not be wise for investors to solely use ESG grade as their lone indicator when deciding on their investment choices. Investors can certainly take a companies ESG rating into account when selecting an investment but factors such as Dividend Payout Ratio, Overall Investment Need, Time Horizon of the investor, Risk factor of the investor, Volatility of the stock/sector, and the overall stock market evnivornment need to be addressed in tandom with ESG grade when detmining the viability of a stock for a particular investor. 

This may be due to a lack or regulation within ESG grading itself as there is currently no standarized grading system for ESG, this can lead to varying data depending on what grading source you use.



# Resources
