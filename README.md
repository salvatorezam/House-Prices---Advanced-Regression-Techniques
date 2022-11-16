# House-Prices---Advanced-Regression-Techniques

The showcased work consists in the Kaggle competition __[House Prices - Avanced Regression Techniques]([http://url](https://www.kaggle.com/competitions/house-prices-advanced-regression-techniques))__ where the challenged are asked to perform a predictive analysis on the market value of real estate assets on the basis of a number of descriptive variables regarding a variety of the properties' characteristics, which affect their sale price in different measures.

![banner](./imgs/housesbanner.png)

The provided __[dataset](http://jse.amstat.org/v19n3/decock.pdf)__ (De Cock, 2011) is composed of `csv` files containing information on the housings of the city of __[Ames](https://www.google.com/maps/place/Ames,+IA,+USA/@42.0258192,-93.6964163,12z/data=!3m1!4b1!4m5!3m4!1s0x87ee70624634a06b:0x273156083cc75200!8m2!3d42.0307812!4d-93.6319131)__, in the Iowa U.S. state. In addition to the dataset, a detailed __[description](https://www.kaggle.com/competitions/house-prices-advanced-regression-techniques/data)__ of the individual fields is given:

- **SalePrice** - the property's sale price in dollars. This is the target variable that you're trying to predict.
- MSSubClass: The building class
- MSZoning: The general zoning classification
- LotFrontage: Linear feet of street connected to property
- LotArea: Lot size in square feet
- Street: Type of road access
- Alley: Type of alley access
- LotShape: General shape of property
- LandContour: Flatness of the property
- Utilities: Type of utilities available
- LotConfig: Lot configuration
- LandSlope: Slope of property
- Neighborhood: Physical locations within Ames city limits
- Condition1: Proximity to main road or railroad
- Condition2: Proximity to main road or railroad (if a second is present)
- BldgType: Type of dwelling
- HouseStyle: Style of dwelling
- OverallQual: Overall material and finish quality
- OverallCond: Overall condition rating
- YearBuilt: Original construction date
- YearRemodAdd: Remodel date
- RoofStyle: Type of roof
- RoofMatl: Roof material
- Exterior1st: Exterior covering on house
- Exterior2nd: Exterior covering on house (if more than one material)
- MasVnrType: Masonry veneer type
- MasVnrArea: Masonry veneer area in square feet
- ExterQual: Exterior material quality
- ExterCond: Present condition of the material on the exterior
- Foundation: Type of foundation
- BsmtQual: Height of the basement
- BsmtCond: General condition of the basement
- BsmtExposure: Walkout or garden level basement walls
- BsmtFinType1: Quality of basement finished area
- BsmtFinSF1: Type 1 finished square feet
- BsmtFinType2: Quality of second finished area (if present)
- BsmtFinSF2: Type 2 finished square feet
- BsmtUnfSF: Unfinished square feet of basement area
- TotalBsmtSF: Total square feet of basement area
- Heating: Type of heating
- HeatingQC: Heating quality and condition
- CentralAir: Central air conditioning
- Electrical: Electrical system
- 1stFlrSF: First Floor square feet
- 2ndFlrSF: Second floor square feet
- LowQualFinSF: Low quality finished square feet (all floors)
- GrLivArea: Above grade (ground) living area square feet
- BsmtFullBath: Basement full bathrooms
- BsmtHalfBath: Basement half bathrooms
- FullBath: Full bathrooms above grade
- HalfBath: Half baths above grade
- Bedroom: Number of bedrooms above basement level
- Kitchen: Number of kitchens
- KitchenQual: Kitchen quality
- TotRmsAbvGrd: Total rooms above grade (does not include bathrooms)
- Functional: Home functionality rating
- Fireplaces: Number of fireplaces
- FireplaceQu: Fireplace quality
- GarageType: Garage location
- GarageYrBlt: Year garage was built
- GarageFinish: Interior finish of the garage
- GarageCars: Size of garage in car capacity
- GarageArea: Size of garage in square feet
- GarageQual: Garage quality
- GarageCond: Garage condition
- PavedDrive: Paved driveway
- WoodDeckSF: Wood deck area in square feet
- OpenPorchSF: Open porch area in square feet
- EnclosedPorch: Enclosed porch area in square feet
- 3SsnPorch: Three season porch area in square feet
- ScreenPorch: Screen porch area in square feet
- PoolArea: Pool area in square feet
- PoolQC: Pool quality
- Fence: Fence quality
- MiscFeature: Miscellaneous feature not covered in other categories
- MiscVal: $Value of miscellaneous feature
- MoSold: Month Sold
- YrSold: Year Sold
- SaleType: Type of sale
- SaleCondition: Condition of sale

Particularly, Kaggle provides the dataset description `data_description.txt` and the files `train.csv` and `test.csv`, those required respectively for the training of the predictive model and the final evaluation (which the score of the competition will be calulated upon). The two `csv` documents have the exact same structure, except of coruse for the **SalePrice** column, not present in `test.csv`, which is associated with the target variable that will need to be predicted by the developed model.

This is a regression problem, where the data preparation and analysis to feed to the training stage happens to be just as crucial, as the model's structure choice itself, as there is a significant number of field for each record (79) and a not so thorough missing/erroneous data imputation, just like the choice of feature that are not relevant in terms of value prediction, may appreciably hinder the efficacy of the used regressors.
