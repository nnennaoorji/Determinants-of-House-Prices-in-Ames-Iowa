# Analyzing the Determinants of House Prices in Ames, Iowa

## Problem Statement 

**What are the key determinants of house prices in Ames, Iowa?** 

In a hypothetical scenario, I have been hired by the City of Ames Assessor’s Office to analyse the Ames Housing dataset. The Office has generated this dataset by nature of its job process as the body responsible for assigning values to all taxable property within Ames' city limits. My task is to generate relevant insights on the determinants of property value in the city, which will be shared with prospective buyers and first-time home owners. The Office is seeking to better educate this class of buyers/home owners and help them make more informed decisions, before and after buying a home. Findings from the analysis are to be published in the City Assessor’s Office “End of Year Digest” and other informational pamphlets/ material relating to mortgages.  


## Data

The Ames Housing dataset is a popular dataset  describing the sale of individual residential property in Ames, Iowa
from 2006 to 2010. A thorough description of the dataset can be found here: [data description](http://jse.amstat.org/v19n3/decock/DataDocumentation.txt).

## Methodology

To address the objectives of the analysis, I specified 3 regression models- OLS, Ridge CV and Lasso CV. Due to the fact that the model is geared towards inference, I avoided data transformation where not absolutely necessary. Feature engineering was similarly conservative, and where applicable, involved dummification and creation of interaction terms. 


## Summary of Results

Generally, results in terms of coefficient maginitude and signage, as well as evaluation metrics were uniform across all 3 models. Interpretation of coefficients from the primary model, the OLS model is presented as follows:

It can be inferred from the model that, all other factors held constant:
* a sq_ft increase in lot area, will increase the sale price of a home by USD 2.4;
* a sq_ft increase in the general living area will increase sale price by USD 94.9;
* A regular shaped lot, relative to an irregular shaped lot will add USD 3,833 to sale price;
* Property constructed on a flat/near level land will be USD 7,293 cheaper than one constructed on relatively slopy land;
* A home with at least 1 fireplace will be USD 4,603 more expensive than one that has no fireplace;
* Having a paved driveway, it appears, decreases property value by USD 4,107;
* A one year increase in a property's age, will decrease its value by USD 1,017;
* Having a garage decreases property value by USD 4,457;
* A 2-family conversion building type is USD 350.7 cheaper than a single family detached home;
* A duplex is USD 7,635 cheaper than a single family detached family home;
* A town house (inside unit) is USD 25,582 cheaper than a single family detached home;
* A town house (end unit) is USD 5,380 cheaper than a single family detached home
* A house located near a rail road is USD 17,398 cheaper than one that is not;
* A house located near or adjacent to a feeder, and/or arterial street is USD 6,183 cheaper than 1 that is not;
* A house located near a postive feature such as a park, or a greenbelt, is USD 5,669 more expensive than one that isn't; and
* As the overall quality of construction materials, finishing and the general condition of the home increases along an ordinal scale (1-10), each unit increase adds USD 2,198 to the value of a home.


## Conclusion

> 1. Property size is the most important factor that influences sale price in Ames. For Ames City, the size of living area (above grade) is valued over lot size.
> 2. The quality and condition of a home are fundamental too, and the most important indicator to look out for, is the age of a property.
> 3. Location matters, and it appears negative features have a greater effect on sale price, than positive features do.
> 4. A fireplace is a very important feature that affects sale price. The shape of the lot, and land contour are key as well. 
> 5. End unit town houses cost a lot more than inside unit town houses. 
> 6. For further study, analyzing features by neighbourhood will interesting to generate inferences that can be generalized for other contexts.

## Recommendations

> 1. Prospective home buyers should pay close attention to understand property location variables. What is the property close to? How busy is the street?

> 2. Details such as land contour, whether or not a fireplace is present, are important details to look out for.

> 3. Property size matters, and in Ames, inside space is valued over outside space.

> 4. Spending on a paved driveway and/or a garage may not be profitable.


### References

[](https://towardsdatascience.com/wrangling-through-dataland-modeling-house-prices-in-ames-iowa-75b9b4086c96)
[](https://www.opendoor.com/w/blog/factors-that-influence-home-value)
[](https://www.homelight.com/blog/buyer-are-basements-included-in-square-footage/)
[](https://www.homelight.com/blog/land-appraisals/)
