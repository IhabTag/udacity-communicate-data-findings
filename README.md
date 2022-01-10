# Bikeshare Data - Exploration and Data Findings Communication Project
## by Ihab Tag


## Dataset

The data set details can be found on the official website at https://www.bluebikes.com/system-data as separate zip files for each year month, I've selected and downloaded the compressed data files for 24 months from Jan, 2018 to Dec, 2019. The original compressed files can be found here https://s3.amazonaws.com/hubway-data/index.html.

I've decompressed the individual files, combined them into one 'csv' file to start working with. A compressed version of it is available here https://www.dropbox.com/s/ztdvsrr67o1y15g/boston_2018_2019.zip?dl=0.

## Summary of Findings

- Total count of trips increased significantly in 2019 in compare to 2018 with a total growth nearly equal to 45%.
- The total monthly trips shows unimodal distribution that peaks around summer months.
- It was interesting to notice that there are no great variations in total daily trips count over week days except for slight decrease during weekends.
- There is bimodal distribution of trips over hours over the day with two peaks, the first is at the morning hours around 08:00 AM, and the second is at the evening hours around 05:00 PM.
- The trip durations shows right skewness with outliers detected for values over 5000 seconds, so the plot was zoomed in for values between 0 and 5000 seconds to better visualize and draw a conclusion about trips durations.
- The subscribers count is about 3 folds of the customers count, and the male users are more than 2 folds of females considering that there is a half million users didn't mention their gender, the relationship between users types should be explored further.
- When exploring the age distribution of users, outliers were detected above age of 80 with maximum value of 155 years! which doesn't make sense and may suggest faulty input of users birth year, so age values above 80 were excluded to better understand this variable.
- Anonther interesting observation was that there was a surge in the age distribution around age of 50 years.
- During the early assessment of data set, new features were engineered to give better exploration results through extracting each trip year, month, day of week and hour in the day and adding a new calculated feature of user age at the time of the trip.
- The trip durations shows right skewness with outliers detected for values over 5000 seconds, so the plot was zoomed in for values between 0 and 5000 seconds to better visualize and draw a conclusion about trips durations.
- When exploring the age distribution of users, outliers were detected above age of 80 with maximum value of 155 years! which doesn't make sense and may suggest faulty input of users birth year, so age values above 80 were excluded to better understand this variable.
- The most active hours of the week days tend to be around hours of going to and returning from work, except for Saturday and Sunday weekends where they tend to be from late morning untill evening.
- In subscribers group, the median age is around 30 with females making more trip durations than males, while the customers with median age around 50 years old tend to have the largest trip durations!
- The trips duration and users age have a strong positive correlation.
- Over months, subscribers showed consistency in their median ages and durations of trips they made, while customers have higher age medians and wider ranges and showed tendency towards higher trips durations.
- On November, the median customers ages dropped from around 50 to around 40 years old, I think this is interesting and should be invistigated further to know the cause.
- In general, subscribers constitutes the vast majority of users with male user more than females, but users in customers group tend NOT to mention their gender.


## Key Insights for Presentation

- I've started with the growth in total trips from 2018 to 2019.
- Moved to distribution of total trips over months.
- Then the trip duration charachterstics.
- Then moved to better understanding user segments throgh classification based on gender and user group.
- Then correlating between the user segments and durations of their trips.
- Then tried to find the most active hours in week days to find patterns.
- Then tried to find the correlation between user age and trip duration.
- Then tried to dig deeper in the relationship between user age in different user groups and the change of them over months.
- Finally, tried to find the relationship between trips duration in different groups and the change of them over months.

## Feedback
- I got a positive feedback on the presentation from one of the Data Session Leads.

## Refereneces
- The main idea of converting categorical variables to numerical ranks for easy plotting as a heatmap was adopted from similar plot at https://github.com/juliaYi/Ford-GoBike-Data-Visualization/blob/master/ford_bike_data_analysis.ipynb