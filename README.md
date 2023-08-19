# Zomoto_Restaurant_Clustering_and_Sentiment_Analysis

## Project Summary
This project centers around restaurant clustering and sentiment analysis of customer reviews on the popular online food delivery platform, Zomato, aiming to extract valuable insights and patterns from a diverse set of data. The project encompasses a series of data processing, engineering, and analytical techniques to achieve its objectives.

Initially, the project kicks off with thorough data cleaning and preprocessing steps. These encompass a comprehensive handling of missing values, outliers, and textual data processing to ensure the quality and accuracy of the dataset.

Subsequently, a strategic approach to feature engineering is executed. This phase encompasses a range of techniques such as feature manipulation, feature selection, data transformation, data scaling, dimensionality reduction and Handling imbalance datasets.

The project then delves into cluster analysis, employing both KMeans and Agglomerative clustering techniques. The determination of the optimal number of clusters is achieved through a combination of the elbow method and silhouette scores.

A significant component of the project revolves around conducting sentiment analysis on the customer reviews. Preliminary results indicate that approximately 82.5% of the sentiments are positive, while the remaining 17.5% reflect negative sentiments.

In conclusion, this project exemplifies the utility of clustering and sentiment analysis in gaining a more profound comprehension of restaurant data on Zomato. The insights procured from the analysis can be of immense benefit to both restaurants and customers in making informed decisions. Furthermore, the project can be extended to other cities or even countries to gain insight into the eating habits and preferences of individuals in different regions.

## Notebook Breakdown
* Business Problem Analysis
  
* Data Collection
  
* Data Cleaning and Preprocessing
  * Handing Missing Value, Outliers and duplicate rows.
     
* Exploratory Data Analysis
   
* Hypothesis Testing
  
* Feature Engineering
  *  Textual Data Preprocessing
     * Expand Contraction, Lower Casing, Removing Punctuations, Stopwords, URL, White Space and digit from Reviews, Tokenization, Lemmatization, Text Vectorization.
     * Feature Manipulation & Selection
     * Data Transformation by log10
     * Data Scaling by StandardScaler
     * Dimesionality Reduction by PCA
     * Data Splitting
     * Handling Imbalanced Dataset by SMOTE
       
* ML Model Implementation
  
* Conclusion


## Conclusion

### **<font color = 'red' > EDA Insight**

#### **<font color = 'blue' > Highly Rated & Low Rated:**

* AB's - Absolute Barbecues and B-Dubs are top-rated.
* Shanghai Chef 2 and Hitech Bawarchi Food Zone have lower ratings.

#### **<font color = 'blue' > Expensive & Affordable:**

* Collage, Feast-Sheraton Hyderabad Hotel, and 10 Downing Street are expensive.
* Mohammedia Shawarma, Amul, and KS Bakers are affordable.

#### **<font color = 'blue' > Customer Sentiments:**

* Most customers rate Zomato restaurants with 4 to 5 stars.

#### **<font color = 'blue' > Engagement Patterns and Review Times:**

* May and July see the highest reviews, while June has less engagement.
* Peak review posting time is 11 pm.

#### **<font color = 'blue' > Common Review Keywords:**

* Customers commonly mention food, place, good, service, and taste.

#### **<font color = 'blue' > Price Points:**

* AB's price: 1500, Zara Hi-Fi: 400.

#### **<font color = 'blue' > Popular Cuisines & Tags:**

* North Indian and Chinese are top cuisines.
* "Great Buffets" is a common tag.

#### **<font color = 'blue' > Top Reviewers and Influential Reviewers:**
* Anvesh Chowdary (3000+ reviews) and Raghu are top reviewers.
* Satwinder Singh has the most followers, followed by Foodies Hyderabad.


### **<font color = 'red' > Restaurant Clustering**

#### **<font color = 'blue' > KMeans Clustering :**

**The Restaurants are clustered into 4 clusters** by using KMeans clustering alogirthm with the **Silhouette score of 0.324382**.

![Screenshot 2023-08-19 140933](https://github.com/manish021996/Zomoto_Restaurant_Clustering_and_Sentiment_Analysis/assets/120492463/8c2cb74a-14ff-4d6b-9de9-d2655b6d61b2)



#### **<font color = 'blue' > Agglomerative Clustering :**
**The Restaurants are clustered into 3 clusters** by using Agglomerative Clustering alogirthm with the **Silhouette score of 0.294.**

![Screenshot 2023-08-19 140821](https://github.com/manish021996/Zomoto_Restaurant_Clustering_and_Sentiment_Analysis/assets/120492463/d23d2d91-91e7-46e8-8641-52153008782e)


### **<font color = 'red' > Sentimental Analysis**
**Sentimental Analysis is to classify the review text as positive or negative.** This provided a more detailed understanding of customer feedback and helped to identify specific areas where the service could be improved.

![Screenshot 2023-08-19 134801](https://github.com/manish021996/Zomoto_Restaurant_Clustering_and_Sentiment_Analysis/assets/120492463/05affb31-a888-478c-aa60-880b4304a5db)

#### **<font color = 'blue'> ML Model**
![Screenshot 2023-07-25 125108](https://github.com/manish021996/Zomoto_Restaurant_Clustering_and_Sentiment_Analysis/assets/120492463/f0e68714-5052-4b70-a957-2665109ffe03)

* Among all the models, XGBoost and RandomForest with GridSearchCV model shows the best performance with highest F1_score.
* It outperforms the all other model.
* No sign of overfitting seen.
* Therefore, XGBoost and RandomForest with GridSearchCV is recommended as the top choice.

