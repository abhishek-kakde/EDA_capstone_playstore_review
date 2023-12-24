# EDA_capstone_playstore_review

The rapid proliferation of mobile applications on the Google Play Store has reshaped the digital landscape, necessitating a profound understanding of user preferences, sentiments, and trends. This exploratory data analysis (EDA) project endeavors to unravel the intricate dynamics within the Play Store, shedding light on app categories, user sentiments, and the factors influencing user ratings.

# Objective:
The primary objective of this EDA is to extract actionable insights from the vast repository of Play Store data, providing developers, stakeholders, and researchers with a nuanced understanding of the app ecosystem.

# Methodology:
The analysis involves the examination of a comprehensive dataset encompassing app categories, user reviews, ratings, and sentiments. Techniques such as descriptive statistics, sentiment analysis, and visualization are employed to distill meaningful patterns from the data.

# Input Files:
Play Store Data.csv - It contains the basic details of the app like number of user reviews, ratings, etc.
User Reviews.csv - It contains the user reviews and its sentiment score for the respective app.

# Exploratory Data Analysis?
Exploratory data analysis (EDA) is used by data scientists to analyze and investigate data sets for patterns, and anomalies (outliers), and form hypotheses based on our understanding of the dataset and summarize their main characteristics, often employing data visualization methods. It is an important step in any Data Analysis or Data Science project. It helps determine how best to manipulate data sources to get the answers you need.

EDA involves generating summary statistics for numerical data in the dataset and creating various graphical representations to understand the data better and make it more attractive and appealing.

📖 Steps Involved

After loading the dataset, we can start the exploration but before that, we need to check and see that the dataset is ready for performing several exploration operations or not, so let’s first have a look at the structure and the manner in which the data is organized.

Data Cleaning
Our data set contains a large number of null values in the rating column, so we drop them. Some of the columns have a smaller number of null values, so we replace the null values in these columns with the mode value of that particular column. Our data set also contain the duplicate rows for a single application. We also drop the duplicate rows because the rows contain the identical data. Also drop the rows, which have rating greater than 5.

Data Transforming
From the information of data frame, we can see that all the columns except rating have the object data type but some of the columns like, reviews, size, installs and price have the numerical value. So, we have to transform them in proper data type and also remove the unwanted values from the numerical columns like ‘+’ and ‘,’ from installs and ‘$’ from price. In the size column we have some values in KB and some values in MB, so we transform all the values in MB.

Exploratory Data Analysis
After establishing a good sense of each feature, we proceeded with plotting a pairwise plot between all the quantitative variables to look for any evident patterns or relationships between the features. There is a high variance in the number of installs and in number of reviews. To overcome this problem, we add two new columns to the data frame named: log_installs and log_review, which contain the logarithmic values of installs and review columns, respectively.

Single Variate Analysis
After that we analysis all the columns one by one to examine whether the particular column contain some useful information or not:

Category
We breakdown the apps by category and observe that family and game categories have the maximum number of apps in the play store. Weather, house and home, comics, events, beauty, and parenting are the categories which have a few numbers of apps.

Data wrangling
Apart from this, new column was added to the main data frame, namely, “Income”. This is done to improve simplify the analysis and come up with different meaningful visualizations

Installs
We analysis the install column to observe the effect of size, price, rating, content rating, android version on app installation number. We can analysis that for each and every category number of app installation does not depend on the size. The free apps installed mostly. The apps which can be used by everyone is more installed than the apps which can be used by a particular age group. Rating of mostly installed apps is between 4 and 5.

# Conclusion
In conclusion, this EDA project serves as a comprehensive guide for navigating the Google Play Store landscape. By elucidating user sentiments and preferences, stakeholders can make informed decisions to enhance app quality, user satisfaction, and overall success in the competitive mobile application market.

📚 References
* W3School
* Medium
* Stackoverflow
* Towards data science
* Python libraries documentation
