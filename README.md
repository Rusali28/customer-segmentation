# Customer-segmentation
Using K Means Clustering to form clusters based on market data of customers.


**ABOUT THE DATA**:
This data set has been retrieved from [kaggle.com](https://www.kaggle.com/) for the learning purpose of the customer segmentation concepts , also known as market basket analysis. This is demonstrated by using unsupervised ML technique (KMeans Clustering Algorithm) in the simplest form.

**DESCRIPTION OF DATA:**
We are owing a supermarket mall and through membership cards , we have some basic data about our customers like Customer ID, age, gender, annual income and spending score.
Spending Score is something we assign to the customer based on our defined parameters like customer behavior and purchasing data.

**PURPOSE:**
We own the mall and want to understand the customers like who can be easily converge (clusters) so that the sense can be given to marketing team and plan the strategy accordingly.

**WORKING WITH THE DATA:**

Here is a glimpse of how our data looks like as a DataFrame. (We have set the customer ID as our index)

![Data Table](https://github.com/Rusali28/customer-segmentation/blob/master/visuals/Data%20Table.PNG)


After checking null values, creating a dummy variable for the Gender column and renaming the column names, we come up with this new modified DataFrame.
We convert the Gender column into a Male column, wherein, 1 is for Male and 0 for Female.

![Modified Data Table](https://github.com/Rusali28/customer-segmentation/blob/master/visuals/Modified%20Data%20Table.PNG)


**EXPLORATORY DATA ANALYSIS:**

Firstly, we create a pairplot to figure out all possible relations between the features in our DataFrame.

![Pairplot](https://github.com/Rusali28/customer-segmentation/blob/master/visuals/Pairplot.PNG)



Next, we move on to a countplot to compare the count of our male and female customers.

![Countplot](https://github.com/Rusali28/customer-segmentation/blob/master/visuals/countplot.PNG)

It can be seen from the plot that the count of female customers is more than male customers.



Next, we use distribution plots to check the distribution of Age, Spending Score and Annual Income.

![distplot 1](https://github.com/Rusali28/customer-segmentation/blob/master/visuals/distplot%201.PNG)

![distplot 2](https://github.com/Rusali28/customer-segmentation/blob/master/visuals/distplot%202.PNG)

![distplot 3](https://github.com/Rusali28/customer-segmentation/blob/master/visuals/distplot%203.PNG)


So we see that Age is pretty evenly distributed, with a few outliers.
For Annual Income, we see most of our customers have an average annual income between 15 to 85 k$.
For Spending Scr, quite a few of our customers have been provided with a spending score between 40 to 60.


Now, we go through a few overlapping histograms using FacetGrid, to compare the gender based behavior for each of the features. Here, the blue shade is for males and orange for females.

![Facetgrid_Age](https://github.com/Rusali28/customer-segmentation/blob/master/visuals/Facetgrid_Age.PNG)


We see that considering age, except for a few outliers, most of the female buyers are younger in age than males.


![Facetgrid_Annual Income](https://github.com/Rusali28/customer-segmentation/blob/master/visuals/Facetgrid_Annual%20Income.PNG)

There is a similar trend over here. The annual income of female buyers is, on an average lesser than males'.

![Facetgrid_Age](https://github.com/Rusali28/customer-segmentation/blob/master/visuals/Facetgrid_Spending%20Score.PNG)

There is a similar trend over here. The spending score of female buyers is, on an average lesser than males'.







