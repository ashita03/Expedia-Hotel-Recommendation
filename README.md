# Expedia-Hotel-Recommendation

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




  
