# Expedia-Hotel-Recommendation
1.filter train data removing is_booking with 0 value.
2.filter users removing agents\n
3.update column orig_destination_distance with category column to remove null values 
4.Convert object format to date format-srch_ci,srch_co,date_time
5.create new columns -stay_dur,no_of_days_before_booking,current_mon,current_year,srch_ci_day,srch_ci_mon,srch_ci_year,srch_co_mon,srch_co_year
6.Drop date columns -date_time,srch_ci,srch_co,is_booking
7.update orig_destination_distance with label encoding
8.Perform PCA on destination data set
9.Merge updated destination set with train data
10.check for null values and update empty cells with 0
11.Perform correlation with target
12.Modeling : 1. Perform Random Forest classifier.