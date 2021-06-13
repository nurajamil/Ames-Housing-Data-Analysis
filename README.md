# Project 2: Ames Housing Data and Kaggle Challenge

---

### Background

A real estate company that you are working for recently got a new client who wants to purchase a property in a quiet area. You are part of a team that is to provide recommendations on the property that he should purchase that would fulfill his requirement and also earn him a return in the future. 

### Problem Statement

Properties in low density areas tend to have low selling prices. Create a model to identify the features and characteristics of a property that would help to increase the value. 

---

### Executive Summary

This project is based on kaggle data set and covers properties that were sold in 2006-2010. The data is broken down to property-level and includes information of features that each property has. 

Using exploratory data analysis and data visualisations, this project aims to look at the different relationships that drive the property price. Through this, the features that are important will be identified, followed by the strategy to improve the value of the property. 

---

### Data Dictionary

|Feature|Type|Dataset|Description|
|---|---|---|---|
|**MS SubClass**|*categorical*|housing|Identifies the type of dwelling involved in the sale. It takes the value of 20, 30, 40, 45, 50, 60, 70, 75, 80, 85, 90, 120, 150, 160, 180, 190.| 
|**MS Zoning**|*categorical*|housing|Identifies the general zoning classification of the sale. It takes the value of "A", "C", "FV", "I", "RH", "RL", "RP", "RM".| 
|**Lot Frontage**|*float*|housing|Linear feet of street connected to property.| 
|**Lot Area**|*int*|housing|Lot size in square feet.| 
|**Street**|*categorical*|housing|The type of road access to property.| 
|**Alley**|*categorical*|housing|The type of alley access to property.| 
|**Lot Shape**|*categorical*|housing|The general shape of property. It takes the value of "reg", "IR1", "IR2", "IR3".| 
|**Land Contour**|*categorical*|housing|Flatness of the property.| 
|**Utilities**|*categorical*|housing|The type of utilities available.| 
|**Lot Config**|*categorical*|housing|Lot configuration.| 
|**Land Slope**|*categorical*|housing|Slope of property.| 
|**Neighborhood**|*categorical*|housing|Physical locations within Ames city limits.| 
|**Condition 1**|*categorical*|housing|Proximity to various conditions.| 
|**Condition 2**|*categorical*|housing|Proximity to various conditions (if more than one is present).| 
|**Bldg Type**|*categorical*|housing|Type of dwelling.| 
|**House Style**|*categorical*|housing|Style of dwelling.| 
|**Overall Qual**|*categorical**|housing|Rates the overall material and finish of the house.| 
|**Overall Cond**|*categorical**|housing|Rates the overall condition of the house.| 
|**Year Built**|*int*|housing|Original construction date.| 
|**Year Remod/Add**|*int*|housing|Remodel date (same as construction date if no remodeling or additions).| 
|**Roof Matl**|*categorical*|housing|Roof material.| 
|**Roof Style**|*categorical*|housing|Type of roof.| 
|**Exterior 1st**|*categorical*|housing|Exterior covering on house.| 
|**Exterior 2nd**|*categorical*|housing|Exterior covering on house (if more than one material).| 
|**Mas Vnr Type**|*categorical*|housing|Masonry veneer type.| 
|**Mas Vnr Area**|*float*|housing|Masonry veneer area in square feet.| 
|**Exter Qual**|*categorical*|housing|Evaluates the quality of the material on the exterior.| 
|**Exter Cond**|*categorical*|housing|Evaluates the present condition of the material on the exterior.| 
|**Foundation**|*categorical*|housing|Type of foundation.| 
|**Bsmt Qual**|*categorical*|housing|Evaluates the height of the basement.| 
|**Bsmt Cond**|*categorical*|housing|Evaluates the general condition of the basement.| 
|**Bsmt Exposure**|*categorical*|housing|Refers to walkout or garden level walls.| 
|**BsmtFin Type 1**|*categorical*|housing|Rating of basement finished area.| 
|**BsmtFin SF 1**|*float*|housing|Type 1 finished square feet.| 
|**BsmtFin Type 2**|*categorical*|housing|Type 2 finished square feet.| 
|**Bsmt Unf SF**|*float*|housing|Unfinished square feet of basement area.| 
|**Total Bsmt SF**|*float*|housing|Total square feet of basement area.| 
|**Heating**|*categorical*|housing|Type of heating.| 
|**Heating QC**|*categorical**|housing|Heating quality and condition.| 
|**Central Air**|*categorical*|housing|Central air conditioning.| 
|**Electrical**|*categorical*|housing|Electrical system.| 
|**1st Flr SF**|*int*|housing|First Floor square feet.| 
|**2nd Flr SF**|*int*|housing|Second floor square feet| 
|**Low Qual Fin SF**|*int*|housing|Low quality finished square feet (all floors).| 
|**Gr Liv Area**|*int*|housing|Above grade (ground) living area square fee.| 
|**Bsmt Full Bath**|*int*|housing|Basement full bathrooms.| 
|**Bsmt Half Bath**|*int*|housing|Basement half bathrooms.| 
|**Full Bath**|*int*|housing|Full bathrooms above grade.| 
|**Half Bath**|*int*|housing|Half baths above grade.| 
|**Bedroom AbvGr**|*int*|housing|Bedrooms above grade (does NOT include basement bedrooms).| 
|**Kitchen AbvGr**|*int*|housing|Kitchens above grade.| 
|**Kitchen Qual**|*categorical**|housing|Kitchen quality.| 
|**TotRms AbvGrd**|*int*|housing|Total rooms above grade (does not include bathrooms).| 
|**Functional**|*categorical*|housing|Home functionality (Assume typical unless deductions are warranted).| 
|**Fireplaces**|*int*|housing|Number of fireplaces.| 
|**Fireplace Qu**|*categorical**|housing|Fireplace quality.| 
|**Garage Type**|*categorical*|housing|Garage location.| 
|**Garage Yr Bltl**|*int*|housing|Year garage was built.| 
|**Garage Finish**|*categorical*|housing|Interior finish of the garage.| 
|**Garage Cars**|*int*|housing|Size of garage in car capacity.| 
|**Garage Area**|*int*|housing|Size of garage in square feet.| 
|**Garage Qual**|*categorical**|housing|Garage quality.| 
|**Paved Drive**|*categorical*|housing|Paved driveway.| 
|**Wood Deck SF**|*int*|housing|Wood deck area in square feet.| 
|**Open Porch SF**|*int*|housing|Open porch area in square fee.| 
|**Enclosed Porch**|*int*|housing|Enclosed porch area in square feet| 
|**3Ssn Porch**|*int*|housing|Three season porch area in square feet.| 
|**Screen Porch**|*int*|housing|Screen porch area in square feet.| 
|**Pool Area**|*int*|housing|Pool area in square feet.|
|**Pool QC**|*categorical*|housing|Pool quality.| 
|**Fence**|*categorical*|housing|Fence quality.| 
|**Misc Feature**|*categorical*|housing|Miscellaneous feature not covered in other categories.| 
|**Misc Val**|*int*|housing|Dollar value of miscellaneous feature.| 
|**Mo Sold**|*int*|housing|Month Sold (MM).| 
|**Yr Sold**|*int*|housing|Year Sold (YYYY).| 
|**Sale Type**|*categorical*|housing|Type of sale.| 
|**SalePrice**|*int*|housing|Dollar value of the property.| 

---

### Conclusions/ Recommendations

The value of a property is influenced by several factors. These factors include the property size, the location, and the quality of the property(including the state of the kitchen and property exterior). It also includes the number of bathrooms and fireplace and the period since the property was last remodelled.

Based on the model, out of all these factors, the location seems to have the biggest impact on the sale price when it comes to properties in low residential density areas. The added value to a property in low residential density areas in zone 4 (most "prestigious" zone) is much higher than the added value to a property in other areas within the same zone. This is in contrast to zone 1(least "prestigious" zone). A property in a low residential density area in zone 1 has a more negative impact on the selling price than a property in other areas within the same zone. Hence, the client should consider purchasing the property in zone 4 and avoid zone 1. Neighbourhoods in zone 4 includes StoneBr and NRidgHt.

Additionally, purchasing a property in a low residential density area that has a fireplace and more bathrooms adds more value to the property.

Moreover, to increase the value, the home owner should maintain his property in the best possible state. He needs to ensure that the overall state of his property, including the kitchen and the exterior of the property to be in the best state and condition. This could be done by renovating the kitchen or repainting or remodelling the exterior and interior of his home. Should he wish to sell the property in the future, he would need to renovate his property just prior to selling it. This is to avoid inccuring a loss and to earn him the maximum amount of returns. 

---

### Data Source

- [Kaggle Challenge](https://www.kaggle.com/c/dsi-us-6-project-2-regression-challenge/data)