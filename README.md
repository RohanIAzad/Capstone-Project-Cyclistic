# Elevator Pitch
The dataset consists of bike riding data under the bicycle sharing system in the Chicago Metropoltan Area. In this case study, I ANalyzed the riding behavious or casual riders (riders who purchase single-ride or full day passes) and annual member riders as the management wants to know how to design a marketing strategy to convert casual riders into annual members. 


### The data analysis process follows the steps below-
### 1. Ask
### 2. Prepare
### 3. Process
### 4. Analyze
### 5. Share
### 6. Act

# 1. Ask
In the "Ask" stage I made note of what is the business task. The director of maketing wants to know how do the riding pattern of casual riders (riders who purchase single-ride or fullday passes) and annual members so that the marketing team can design a marketing starttegy to convert casual riders into annual members. The marketing director thinks annual members generate more profit for the company compared to the casual riders. 

# 2. Prepare
The "Prepare" phase is concerned with collecting the relevant data that is complete, accurate, consistent, trustworthy, unbiased. Teh data should also be current and teh reference cited.

This data is reliable, original, comprehensive and current as it is made publicli avaialble by Lyft Bikes and Scooters with the permission of the City of Chicago. Personally identifiable information such as credit card numbers has been removed because of data-privacy issues.

# 3. Process
The data is organized month by month from June 2020 to May 2021. 
The data contains information on the type of bicycle being used, at what time did the ride start and at what time did it end, latitude, longitude of the starting and ending location. Also has the whether the user is a casual rider or an annual member,

The data integrity is not satisfied as it has missing values, in some cases "started_at" time was later than "ended_at" although it may be accurate, consistent, trustworthy. 

I used pyhton for processing and cleaning the data.

1. Merged the 12 datasets togethers
2. Looked into misisng values. Teh columsn that did have missing values, I didnot require those for my analysis. That si why did not delete those rows with misisng values. 
3. Checked for duplicate entries. There were no duplicate entries.
4. Looked into the info() of teh dataset. Teh started_ata nd ened_at columsn were not in the correct format. they were strings and no datetime. Used pandas to_datetime() method to convert those to datetime.
5. Extracted "day of the week" and "month" from datetime
6. Noticed that in some cases "started_at" was at a later time than "ended_at". Swapped the entries so that "started _at" and "ended_at" can be swtiched to reflect lower "started_at" and higher "ended_at" time.

# 4. Analysis
I did analysis on -
1. the percentage of casual and member riders in the entire dataset
![1  Total Bike Hires Per Rider category](https://user-images.githubusercontent.com/43137227/166157814-777c0507-eacb-46f3-8ef0-e12411dabe0d.PNG)

2. Total bike hires per month
![2  Total Bike Hires per Month](https://user-images.githubusercontent.com/43137227/166157948-e883ebcc-f706-4c73-8cd2-02476c714548.PNG)






