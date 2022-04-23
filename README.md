# Project 2: Home Value Assessment for Ames, Iowa 

### Problem Statement 

A lovely older couple, Joan and Janice Smith, have decided to purchase a second home in Ames, Iowa, and need help determining which homes would be best for them. Unlike your typical homebuyer, Joan and Janice's main constraints are that they want a home with better privacy, especially a back yard they can spend time in unbothered. I will use linear regression to narrow down a large set of sale data into good and great deals, which can then be used to determine if any house they find currently for sale in Ames is a good deal or not.

### Dataset

For this hypothetical situation, we are using the dataset [Ames Iowa: Alternative to the Boston Housing Data Set](http://jse.amstat.org/v19n3/decock/DataDocumentation.txt). From the description:
>Data set contains information from the Ames Assessor’s Office used in computing assessed values for individual residential properties sold in Ames, IA from 2006 to 2010.

From this dataset we will be using a handful of predictive variables, many of which are engineered from the original data.

##### Data Dictionary

|Feature|Type|Description|
|------|------|------|
overall_qual|Ordinal|1-10 The overall material and finish of the house|
total_overall_sf|Continuous|The combined house and garage square footage|
garage_interact|Continuous|The interaction term of garage square footage and car capacity|
years_interact|Continous|The interaction term of the year the house was built and the year it was remodeled or added onto|
total_full_bath|Numeric|The total number of full bathrooms in the house|
sf_bath|Continous|The interaction term of house square footage and number of full baths|
fence_ord|Ordinal|The quality of the fence, 5 if Good Privacy, 4 if NA, 3 if Good Wood, 0 otherwise|
bldg_type_ord|Ordinal|The type of structure. 5 if Single Family, 0 otherwise|
exter_qual_ord|Ordinal|1-5 The quality of the materials of the exterior|
bsmt_qual_ord|Ordinal|0-5 The height of the basement|
kitchen_qual_ord|1-5 The quality of the kitchen|
lot_config|Nominal|The type of lot: Inside, Corner, Cul-de-sac, Frontage 2 Sides, Frontage 3 Sides|
neighborhood|Nominal|The neighborhood in Ames the house is located in|

### Overview
The main goal of this analysis is to create a model which will reliably predict sale price and to create a second model which is optimized for the privacy features my clients find most important. Using these two models I can pull out which houses are good deals in general and which are even better deals given their specific needs. From there, my clients would be able to use these models to generalize to houses they see for sale on the market, and determine quickly and efficiently if those are good deals for them.

### Conclusions
There are many more houses in Ames that are overpriced for my clients than there are good deals. Of the over 2000 data points given, only 25 fell within the good and great deal brackets for their contraints. By having my clients look over these listings, and share any positive or negative features that stand out to them, I can further optimize my models on the current data and create even better predictions for them in the future. Ultimately, this model should really streamline the process for them, allowing them to focus more on the subjective qualities of the home, and less on whether they are getting a fair market price.
