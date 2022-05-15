# Pyberhood
## Project Overview
Create a NASDAQ screener to find stable investments for the week.

### Purpose
Gather NASDAQ's stock data from APIs over the weekend (free version takes ~ 26 hours) for a specified date range. Then clean these results and export 3 csv's containing all data, the smallest winner and the smallest loosers. Finally we'll remove any outliers and vizualize the results.

## Analysis
First, create a field to input what kinds of data to gather and from where. While importing the data, make sure to print and store any unavailible tickers. <br />
<img width="1343" alt="Screen Shot 2022-05-15 at 11 42 29 AM" src="https://user-images.githubusercontent.com/79609464/168486542-40a6f2ce-a812-4020-8fe8-34568fb1d228.png"> <br />

Then, store retieved data in a new data frame (some stocks aren't traded on everyday), hence they won't have a five element list. <br />
<img width="1028" alt="Screen Shot 2022-05-15 at 11 44 53 AM" src="https://user-images.githubusercontent.com/79609464/168486623-521ff851-69d7-4572-affa-d20f06a1a7cf.png"> <br />

After clean the results, store them in 3 seprate dataframes, and sort by the week's performance. <br />
<img width="1329" alt="Screen Shot 2022-05-15 at 11 48 21 AM" src="https://user-images.githubusercontent.com/79609464/168486730-cdcd147d-51bf-4100-9b40-c7f4974f8181.png"><br />



### Centering Data
The data is skewed by volatile stocks, so remove any outliers.<br />
<img width="1386" alt="Screen Shot 2022-05-15 at 11 31 20 AM" src="https://user-images.githubusercontent.com/79609464/168486041-1743f94d-cd48-45b6-b482-435a7f9c5566.png"><br />
<img width="841" alt="Screen Shot 2022-05-15 at 11 49 30 AM" src="https://user-images.githubusercontent.com/79609464/168486801-46a11e46-8dab-4727-a825-647a35d01419.png"><br />

Finally, graph the week's highest price vs its performance and use color to vizualize the volatility<br />
<img width="1252" alt="Screen Shot 2022-05-15 at 12 23 51 PM" src="https://user-images.githubusercontent.com/79609464/168488051-f04f7c11-5a24-4b90-890a-f170cedd1762.png">


### Challenges and Difficulties Encountered


## Results


## Summary

