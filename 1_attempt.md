# Claims
1. prices are rising 
2. City 2 is more expensive
# Questions and variables
1.Question for claim 1: is the price on the last date higher then the first date, for each item individually in both cities?
variables needed: item, price,city, date
2. Question for claim 2: for each item, is the price higher in city 2 than in city 1 at all dates?
variables needed:date, price, city, item
# predictions
shape(rows * columns): 90*6
distinct items:4
distinct dates:1-1-26 --1-6-26 (across 6 months, weekly span)