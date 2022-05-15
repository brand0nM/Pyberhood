# Pyberhood
## Project Overview
Create a NASDAQ screener to find stable investments for the week.

### Purpose
Gather stock data from APIs over the weekend (free version takes ~ 26 hours) for a specified date range. Then clean these results and export 3 csv's containing all the data, the smallest winner and the smallest loosers. Finally we'll remove any outliers and vizualize the results.

## Analysis
First, create a field to input what kinds of data to gather and from where. While importing the data, make sure to print and store any unavailible tickers. <br />
<img width="1343" alt="Screen Shot 2022-05-15 at 11 42 29 AM" src="https://user-images.githubusercontent.com/79609464/168486542-40a6f2ce-a812-4020-8fe8-34568fb1d228.png"> <br />

Then, store retieved data in a new data frame (some stocks aren't traded on everyday), hence they won't have a five element list. <br />
<img width="1028" alt="Screen Shot 2022-05-15 at 11 44 53 AM" src="https://user-images.githubusercontent.com/79609464/168486623-521ff851-69d7-4572-affa-d20f06a1a7cf.png"> <br />

After clean the results, store them in 3 seprate dataframes, and sort by the week's performance. <br />
<img width="1329" alt="Screen Shot 2022-05-15 at 11 48 21 AM" src="https://user-images.githubusercontent.com/79609464/168486730-cdcd147d-51bf-4100-9b40-c7f4974f8181.png"><br />

### Centering the Data
The data is skewed by volatile stocks, so remove any outliers.<br />
<img width="1386" alt="Screen Shot 2022-05-15 at 11 31 20 AM" src="https://user-images.githubusercontent.com/79609464/168486041-1743f94d-cd48-45b6-b482-435a7f9c5566.png"><br />
<img width="841" alt="Screen Shot 2022-05-15 at 11 49 30 AM" src="https://user-images.githubusercontent.com/79609464/168486801-46a11e46-8dab-4727-a825-647a35d01419.png"><br />

### Highest Price vs Performance with Color Volatility
<img width="1252" alt="Screen Shot 2022-05-15 at 12 23 51 PM" src="https://user-images.githubusercontent.com/79609464/168488051-f04f7c11-5a24-4b90-890a-f170cedd1762.png">
-The more expense the stock price, the less volatile it's performance
--Exceptions could be attributed to negative publicity caused many to sell.
-The last week weighted average is slowly increasing in a volatile manner.

### Challenges and Difficulties Encountered
Since we were using the free version on polygon's stock api, gathering data took around a day; a few times my computer was acidentally unplugged and I lost all progress. Another difficulty was accurately interpreting the results without also catogrizing each stock into its sector. To further improve this project we could scrape sector data, or find another API to populate. Then I we could vizualization each sector and modifiying our existing graph to color by sector and size by volatility. Having this data would allow for a more thorough analysis of how the stock market is actually performing.

## Results
One can enable magic commands in the vizualization notebook to view specific points of interest; From the volatility csv we can filter based on desired paramaters to choose investments. Additionally the smallest winner's and looser's csv can be viewed to find investments; once selected cross refencencing the volatility csv would help determine if the investment makes sense.

## Summary
We've successfully created a weekly stock screener to vizualize NASDAQ's performance as a whole and find stable investments. 
