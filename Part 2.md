# Discussion topics part 2

## The AWS-lesson

1. Is it a good idea to be using Python and Jupyter notebooks? Are there any alternatives like Julia, R, Java, C#, …? <hr> Python and Jupyter notebooks are excellent choices for many data-related tasks due to their ease of use and rich ecosystem. However, alternatives like Julia, R, Java, and C# may be more suitable depending on your specific requirements and preferences. It's often a good idea to be familiar with multiple languages and tools to choose the best one for a given project.

2. Amazon has some managed services that provide AI-services without the need for any real understanding of the technology involved. Will they preform better than a model that we can make ourselves? What are the [dis]advantages of using them? <hr> The main advantages are: easy of use, quick deployment, scalability and amazing integration. The disadvantages are that there is limited customization and high costs.
Choosing between managed services and custom models depends on project requirements, expertise, budget, and customization needs. A hybrid approach, using both managed and custom solutions, is also a viable option in many cases. 

    ![](files/2023-04-11-18-35-30.png)

3. Give an example of supervised and unsupervised learning when using a file with all data about students (grades, but also age, shoe size, family situation, …).  <hr> Supervised learning involves training a model to make predictions or classifications based on labeled data. In this case, we can consider a scenario where you want to predict a student's final exam score based on various features like age, shoe size, and family situation. 
Unsupervised learning involves finding patterns or relationships in data without labeled outcomes. In this case, we can consider a scenario where you want to group students into clusters based on similarities in their age, shoe size, and family situation.
Unsupervised learning helps you uncover hidden patterns or groupings in your data without prior labels, which can be useful for segmentation or exploratory analysis.


4. We have a file of student grades and how much they studied for a test. We want to predict their test scores. Explain the difference between binary classification, multi-label classification and regression in this context.<hr> The choice between binary classification, multi-label classification, or regression in your context depends on the nature of the outcome you want to predict. If you are interested in pass/fail outcomes, use binary classification. If you want to categorize performance into multiple labels, use multi-label classification. For predicting exact test scores, use regression.

 
5. Can we use AI to do feature engineering? Is it regularly done this way? <hr> Yes, we can! AI techniques, particularly automated machine learning (AutoML) and deep learning, can be used for feature engineering, and it's becoming increasingly common in data science and machine learning workflows. Feature engineering is the process of selecting, creating, or transforming features (variables) from raw data to improve the performance of machine learning models.

6. Explain over- and underfitting in the context of multi-label classification. <hr>
Overfitting occurs when a model learns the training data too well, capturing noise and random fluctuations in the data rather than just the underlying patterns. As a result, the model performs exceptionally well on the training data but fails to generalize to unseen or test data. Underfitting occurs when a model is too simple to capture the underlying patterns in the data. In this case, the model's performance is poor on both the training data and the test data because it fails to learn essential relationships.
Very important is finding the right balance between them. You want your model to generalize well to unseen data while capturing meaningful patterns in the training data.


## The powerpoint and exercises

1. The powerpoint states: "The model should generalize to unseen data if you are using it to predict. If it’s just to explain the data overfitting isn’t a problem." Explain! <hr> When the primary goal of your machine learning model is to make accurate predictions on new, unseen data, generalization is crucial. Overfitting, which occurs when a model memorizes the training data and fails to generalize, can be a severe problem. In predictive modeling, overfitting can lead to poor performance because the model will not perform well on data it hasn't encountered during training. It might make overly specific predictions that don't hold true for new data points. 
1. To get rid of outliers, we simply look at the values and delete the row with the highest value for every column. Or is there a better way?<hr> Removing outliers by simply deleting rows with the highest value for every column is not generally a recommended approach because it can lead to a loss of valuable information and potentially bias your data. Outliers should be handled with more thoughtful and data-driven methods. A better way is to first identify outliers, then understand the context and afterwards you can transform the data.
1. Why does the Z-score doesn't matter in a column that is used in one hot encoding? <hr> Z-scores are not applicable or meaningful for one-hot encoded columns because they are designed for continuous, normally distributed data. One-hot encoding is specifically used for categorical data, where the notion of standard deviations and distances from the mean doesn't have relevance. When working with categorical data, it's more important to focus on appropriate encoding techniques and handling the categorical variables effectively within your machine learning or statistical analysis.
1. What is scaling/normalization of data? <hr> Scaling refers to the process of transforming the values of a feature to lie within a specific range while normalization is often used interchangeably with min-max scaling, but it can also refer to other data transformations that adjust the data to follow a specific distribution or remove skewness.





