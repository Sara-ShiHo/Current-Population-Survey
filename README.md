# Current-Population-Survey

## Motivation

Why calculate unemployment rates using python code? 

* Integrity - we are calculating the unemployment rate directly from same source that the BLS uses
* Customization - we can accordingly calculate the unemployment rate for different segments of the population that we are interested in

Is there anything to be concerned about?

* Seasonality - the code in this repo only calculates **Non-Seasonally-Adusted** unemployment rate. To factor in seasonality, you would have to download historical data as well as the current monthly data. 
* Small sample size - technically, you can use this code to calculate the unemployment rate for a small, specific subset of the population. But take into consideration that the CPS only surveys 60,000 households per month. The more specific your query, the smaller your subset - subsequently your results are less likely to be representative of the actual U.S. population (See Law of Large Numbers).