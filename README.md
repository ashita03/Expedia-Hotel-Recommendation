# Expedia-Hotel-Recommendation

## About -

Employing various machine learning models like Random Forest Classifier, Keras, and Support Vector Machine, we endeavored to identify the optimal model for accurately categorizing recommendations into the correct cluster among 100 target clusters. In addressing the challenge posed by a large dataset comprising 37 million rows, we adopted three distinct strategies to reduce dataset size while ensuring the retention of crucial features through Principal Component Analysis.

These approaches included: i) utilizing a dataset of randomly selected 50,000 unique users, ii) working with a dataset focusing on the top 10 clusters, and iii) implementing clustering as a pre-processing step, involving the creation of an optimal number of clusters derived from the target clusters. Notably, the third method emerged as the most effective, particularly in conjunction with Keras, showcasing outstanding accuracies of 87.1% and 93% for 10 and 20 clusters, respectively. This successful outcome underscores the importance of strategic dataset reduction and pre-processing techniques in overcoming the challenges posed by large datasets and enhancing the accuracy of machine learning models.

## Steps followed - 
- Filter train data removing is_booking with 0 value.
- Filter users removing agents
- Update column orig_destination_distance with category column to remove null values 
- Convert object format to date format-srch_ci,srch_co,date_time
- Create new columns -stay_dur,no_of_days_before_booking,current_mon,current_year,srch_ci_day,srch_ci_mon,srch_ci_year,srch_co_mon,srch_co_year
- Drop date columns -date_time,srch_ci,srch_co,is_booking
- Update orig_destination_distance with label encoding
- Perform PCA on destination data set
- Merge updated destination set with train data
- Check for null values and update empty cells with 0
- Understand correlation with Target variable
- To deal with the large dataset and limited computational power, 3 major methods of reducing the dataset were used:
  - Data of random 50,000 unique users
  - Data of top 10 clusters
  - Creating clusters of the target variable (merging multiple clusters into 1 to reduce the total number of target clusters)    
- Train & Testing

## Results
![Results](https://github.com/ashita03/Expedia-Hotel-Recommendation/blob/main/images/results.jpg)



  
