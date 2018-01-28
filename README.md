# Data Analyst Internship Challenge Summer 18 Shopify

1. What could be going wrong with our calculation (and correct it).

   The mean is too large because it is greatly influenced by outliers ( shop id 42 order amount = 11,990,176.0 and shop id 78 order amount = 2,263,800 ) that have huge order amounts. 

   Hence choosing mean as a metric to represent AOV is misleading.


2. What may be a better way to evaluate this data?

   So we calculate mean, median, standard deviation, etc and plot histogram, xy plot and  box plot using matplotlib to better understand the data
   
   Mean:  3145.128
   Median:  284.0
   Standard deviation: 41278.4108884
   Minimum: 90.0
   Maximum: 704000.0
   Standard error: 583.823270363

   After careful analysis, I have come to a conculsion that median would be the best metric to evaluate AOV


3. What other data would be helpful in measuring if a shop is successful?
   
   First lets add the order_amount for each shop_id and store them in a dictionary. Now we would have total_order_amounts for all respective shop_ids (1-100). Then we can store the order_amounts corresponding to each shop_id in a list and do exploratory analysis on that.

   we find again mean to be a bad metric (greatly influenced by outliers) to measure success of a shop, hence we choose median to measure if a shop is successful or not.

   Mean:  157256.4
   Median:  14887.5
   Standard deviation: 1210121.56805
   Minimum: 6840.0
   Maximum: 11990176.0
   Standard error: 121621.793695

   After comparing all shop_ids & their respective order_amounts WITH median, we found out that out of 100 shops, 50 shops were successful since their order_amounts were found to be greater than or equal to median.

