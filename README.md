# Sales Predictions

**Task:** Analyze dataset provided by the retailer to determine item and/ or outlet characteristics that play crucial roles in predicting sales.

**Purpose:** Leverage machine learning to help the retailer make predictions about future sales based on the data provided.

**The code:** Using Colaboratory and written in the python language, this project is broken down into four sections, each serving an important function in analysis of the data and meeting the objectives of this project.
1.	Establishment of Tools and Importing the Data
2.	Preprocessing the data
>  a.	Ensures the data is ready for analysis and modeling
3.	Data Visualization 
>  a.	Exploratory Visualization
>>    i.	Extract critical information
>  b.	Explanatory Visualization
>>    i.	Generate presentation ready graphics
5.	Modeling sales and Evaluation their performance
>  a.	Linear Regression Model (sklearn)
>  b.	Random Forest Regression Model (sklearn)

**Findings:** Based on analysis of the dataset and the below determinations on characteristics’ importance, I was able make the recommendation for shifting 955 items with low visibility and high MRP to higher visibility while shifting 3,138 items with high visibility and low MRP to low visibility. This move has the potential to increase total sales from ~18.6M to ~22M, an increase of ~3.4M.
-	Factors with limited impact on sales:
>  o	 Item Weight
>  o	Item Fat Content
>  o	Item Type
>  o	Outlet Establishment Year
>  o	Outlet Location Type
-	Factors with real impact on sales
>  o	Item Visibility
>  o	Item MRP
>  o	Outlet Size
>  o	Outlet Type

![New Visibility](https://user-images.githubusercontent.com/94806791/150704057-072e8f95-f351-4e78-b673-d98e8aa21b4c.png)
This graphic shows the value of the high MRP items that currently have too low visibility

**Modeling:** I testing both a Linear Regression Model and a Random Forest Regression Model. I attempted 6 different hyperparameter tunings on the Random Forest Regression Model and was able to achieve a r2 score on the training dataset of 0.68 and a r2 score on the testing set of 0.59. Both the Linear Regression Model and all other variation of the Random Forest Regression Model resulted in overfitting to the training set or lower scores.

**Recommendation:** My recommendations to the retailer are
1.	Continue working with me in order to implement the Random Forest Regression Model to predict future sales. 
2.	Reduce visibility for the 3,138 items with low MRP (itemized excel provided)
3.	Increase visibility for the 955 items with high MRP (itemized excel provided)
