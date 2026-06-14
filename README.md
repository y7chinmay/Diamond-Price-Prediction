# Diamond-Price-Prediction
PRICE PREDICTION OF DIAMONDS: REGRESSION

1. IMPORTING LIBRARIES
2. LOADING DATA
3. DATA PREPROCESSING
4. MODEL BUILDING
-------------------------------------------------------------------------------------------------------------------------------------------------------------------
**Loading Data**

This classic dataset contains the prices and other attributes of almost 54,000 diamonds. There are 10 attributes included in the dataset including the target ie. price.
-------------------------------------------------------------------------------------------------------------------------------------------------------------------
Feature description:

price price in US dollars (326--18,823)This is the target column containing tags for the features. 

The 4 Cs of Diamonds:-

carat (0.2--5.01) The carat is the diamond’s physical weight measured in metric carats.  One carat equals 1/5 gram and is subdivided into 100 points. Carat weight is the most objective grade of the 4Cs. 

cut (Fair, Good, Very Good, Premium, Ideal) In determining the quality of the cut, the diamond grader evaluates the cutter’s skill in the fashioning of the diamond. The more precise the diamond is cut, the more captivating the diamond is to the eye.  

color, from J (worst) to D (best) The colour of gem-quality diamonds occurs in many hues. In the range from colourless to light yellow or light brown. Colourless diamonds are the rarest. Other natural colours (blue, red, pink for example) are known as "fancy,” and their colour grading is different than from white colorless diamonds.  

clarity (I1 (worst), SI2, SI1, VS2, VS1, VVS2, VVS1, IF (best)) Diamonds can have internal characteristics known as inclusions or external characteristics known as blemishes. Diamonds without inclusions or blemishes are rare; however, most characteristics can only be seen with magnification.  

Dimensions

x length in mm (0--10.74)

y width in mm (0--58.9)

z depth in mm (0--31.8)

**depth total depth percentage = z / mean(x, y) = 2 * z / (x + y) (43--79)**
The depth of the diamond is its height (in millimetres) measured from the culet (bottom tip) to the table (flat, top surface).

**table width of the top of the diamond relative to widest point (43--95)**

A diamond's table refers to the flat facet of the diamond seen when the stone is face up. The main purpose of a diamond table is to refract entering light rays and allow reflected light rays from within the diamond to meet the observer’s eye. The ideal table cut diamond will give the diamond stunning fire and brilliance.
-------------------------------------------------------------------------------------------------------------------------------------------------------------------
**Data Preprocessing**
Steps involved in Data Preprocessing

**Data cleaning**
Identifying and removing outliers
Encoding categorical variables
-------------------------------------------------------------------------------------------------------------------------------------------------------------------
**Model Building**
Steps involved in Model Building

Setting up features and target
Build a pipeline of standard scalar and model for five different regressors.
Fit all the models on training data
Get mean of cross-validation on the training set for all the models for negative root mean square error
Pick the model with the best cross-validation score
Fit the best model on the training set and get
-------------------------------------------------------------------------------------------------------------------------------------------------------------------
**Testing the Model with the best score on the test set**

In the above scores, XGBClassifier appears to be the model with the best scoring on negative root mean square error. Let's test this model on a test set and evaluate it with different parameters. 
