# Stock Yearly Earnings Analysis and Code Performance
## Overview
### The purpose of this analysis is first to analyze stock market yearly returns for a select set of stocks for the years 2017 and 2018; And second is to attempt to refactor initial code format in order to streamline and enhance performance when running the code.
## Results: Stock Analysis
### This analysis looked at 12 stock market tickers ($AY, $CSIQ, $DQ, $ENPH, $FLSR, $HASI, $JKS, $RUN, $SEDG, $SPWR, $TERP, & $VSLR) over the years 2017 and 2018 to guage their total volume traded and return for the requested year. In 2017, 11 of the 12 tracked tickers had a positive yearly return with the highest being $DQ at 199.4% and the only loss being $TERP at -7.2%. However, for the year 2018. 10 of the 12 tickers suffered losses for the year with the greatest loss being $DQ at -62.6%. The 2 gainers of 2018, $ENPH and $RUN, rose 81.9% and 84% respectively. This shows that the best time to sell would have been in 2017 and possibly buy again in 2018.
## Results: Code Performance
### When the analysis code was originally written, it had an average run time of about 1 second for each year, and also stuttered slightly when filling in the sheet. This lead to an unpleasant user experience and if used on a much larger data set could have exponentially increased run time.
![2018 Refactored Code Performance Time](https://user-images.githubusercontent.com/102704559/164936515-840b199d-118d-4f55-80f7-375b027ff2d3.PNG)
![2018 Original Code Performance Time](https://user-images.githubusercontent.com/102704559/164936510-22955a12-8bd6-4ece-8aa2-fe80b0d20b07.PNG)
