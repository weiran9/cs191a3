# ps4 Index
## what is PPP?
PPP is a kind of spatial price index, which can eliminate the price differences among economies by measuring the purchasing power of their currencies, so that the international comparison of GDP can be based on the actual volume of goods. Theoretically, its comparison results are more objective and scientific than the exchange rate method.
## why ps4?
The ps4 is a home game console released by Sony in North America from November 15, 2013. Despite its age, it is still being produced and sold in 2022, and on December 31, 2019, cumulative worldwide sales of the PS4 have surpassed 106 million units. It is widely known and sold in almost every country in the world, which is why I chose it for this project
## the creation of index
### 1. Scrape PS4 pricing data from website
I found ps4 price data for over 100 countries on https://www.psdevwiki.com/ps4/Prices which was enough for me to complete the project. I used the method from the class to import the data from the website into the table.
### 2. clean up data
I removed the information for Chile and Kuwait from the table, as they did not import correctly, and corrected the information for Canada. Then used the split function to extract the numbers and currency symbols from the table separately 
### 3. change all currency to USD
I scrape over their country code from currencyscoop.com and add the country code to my own form for the next currency conversion. Then I use a for loop to iterate through all the countries on my table to convert each country's currency to USD using the currencyscoop.com API.
### 4.calculate difference between American price and price from other countries
I took the converted prices and subtracted the US PS4 prices to calculate the difference between them, simply subtracting 399.00 from each price.
