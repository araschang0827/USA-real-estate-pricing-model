# 🏠USA Real Estate Pricing Model🏠
## I.Brief Description of the Topic
After the pandemic, people have been living in homes for a long time, as a result, their requirements for living quality have also increased invisibly. In the eyes of American real estate buyers, buying houses with larger living space has become a trend. However, with the fluctuation of interest rates and housing prices, as well as the interaction of geographical factors, housing prices have become unpredictable, and this unknown has also formed a strong resistance to those who want to buy real estate. Therefore, we hope that through the analysis of the interaction between the internal structure of the house and the locality, we can establish a convenient and applicable house valuation model for real estate buyers in the United States.
## II.Brief Description of the Dataset
The data for the analysis was obtained from Kaggle, a data modeling and data analysis competition platform owned by Google LLC. After scouring the platform for this research topic, we decided to use USA Real Estate Dataset.The data in this dataset is collected by researchers using python to capture the housing transaction data on the US real estate transaction website realtor.com, and the data format is a CSV file. There are more than 200,000 housing information in USA Real Estate Dataset, which contains seven kinds of qualitative data of houses in each transaction: status, full address, street, city, state, zip code, sold date, and five kinds of quantitative data: price, bed, bath, acre lot, house size. After screening out some invalid data, we used the remaining 170,000 pieces of data to perform machine learning regression analysis. In this analysis, we will use the variable "price" as the observed value $y$, and make a model under different "states" (nine states in total), enter "number of bed bedrooms", "number of bathroom bathrooms" and "house size". At the end, we use this model to design an interactive model of expected house price that can interact with users.
## III.Data Processing
We first use the "house area" in USA Real Estate Dataset as a single 𝑥 variable, corresponding to the $y$ variable "price” as a simple regression model $y=x_1B_1+B_0$ , as shown in the figure below, it can be seen that both $R$(0.024) and $R^2$ (0.00056) are very low, indicating that the explanatory power of its single variable is low.
![alt text](https://github.com/araschang0827/USA-real-estate-pricing-model/blob/master/simple%20regression.png?raw=true)