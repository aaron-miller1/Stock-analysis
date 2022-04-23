# Stock Yearly Earnings Analysis and Code Performance
## Overview
### The purpose of this analysis is first to analyze stock market yearly returns for a select set of stocks for the years 2017 and 2018; And second is to attempt to refactor initial code format in order to streamline and enhance performance when running the code.
## Results: Stock Analysis
### This analysis looked at 12 stock market tickers ($AY, $CSIQ, $DQ, $ENPH, $FLSR, $HASI, $JKS, $RUN, $SEDG, $SPWR, $TERP, & $VSLR) over the years 2017 and 2018 to guage their total volume traded and return for the requested year. In 2017, 11 of the 12 tracked tickers had a positive yearly return with the highest being $DQ at 199.4% and the only loss being $TERP at -7.2%. However, for the year 2018. 10 of the 12 tickers suffered losses for the year with the greatest loss being $DQ at -62.6%. The 2 gainers of 2018, $ENPH and $RUN, rose 81.9% and 84% respectively. This shows that the best time to sell would have been in 2017 and possibly buy again in 2018.

![2017 Stock Analysis Results](https://user-images.githubusercontent.com/102704559/164937105-f99290bb-dc5b-4dac-a769-d6e3bd2a52a0.PNG)
![2018 Stock Analysis Results](https://user-images.githubusercontent.com/102704559/164937116-edb368fb-5d3b-495f-a7f2-0040e6b40e34.PNG)


## Results: Code Performance

### When the analysis code was originally written, it had an average run time of about 1 second for each year, and also stuttered slightly when filling in the sheet. This lead to an unpleasant user experience and if used on a much larger data set could have exponentially increased run time.

![2017 Original Code Performance Time](https://user-images.githubusercontent.com/102704559/164936534-47c3079d-5ee2-4266-aebc-73e9ed1504a8.PNG)
![2018 Original Code Performance Time](https://user-images.githubusercontent.com/102704559/164936510-22955a12-8bd6-4ece-8aa2-fe80b0d20b07.PNG)

### In order to improve upon run time, I edited the 'startingPrice' and 'endingPrice' arrays to take in a variable, in this case being the specific ticker from 'tickerIndex', as well as changed the original nested for loop into a single for loopThis allowed for the prices of each index to be ran and stored more efficiently before moving onto the next line in the process since the following for loop could pull the stored data from each of the arrays for each ticker individually instead of all at once. 

![Refactored_Output Arrays](https://user-images.githubusercontent.com/102704559/164942656-0a06d0cb-5202-4175-bb2a-03041b8e6762.PNG)

### This lead to a dramatic increase in the over all performance of the code, with each year running in approximately 0.1 seconds.

![2017 Refactored Code Performance Time](https://user-images.githubusercontent.com/102704559/164942681-e6d2e259-7ac2-45b5-8d14-ba2d82984c69.PNG)
![2018 Refactored Code Performance Time](https://user-images.githubusercontent.com/102704559/164942684-4b50781b-9864-48f4-b5b1-13257c1da4f7.PNG)

