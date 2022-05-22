# Elevator Pitch
The dataset consists of bike riding data under the bicycle sharing system in the Chicago Metropoltan Area. In this case study, I Analyzed the riding behavious of casual riders (riders who purchase single-ride or full day passes) and annual member riders as the management wants to know how to design a marketing strategy to convert casual riders into annual members. 


### The data analysis process follows the steps below-
### 1. Ask
### 2. Prepare
### 3. Process
### 4. Analyze
### 5. Share
### 6. Act

# 1. Ask
In the "Ask" stage I made note of what is the business task. The director of maketing wants to know how do the riding pattern of casual riders (riders who purchase single-ride or fullday passes) and annual members differ so that the marketing team can design a marketing starttegy to convert casual riders into annual members. The marketing director thinks annual members generate more profit for the company compared to the casual riders. 

# 2. Prepare
The "Prepare" phase is concerned with collecting the relevant data that is complete, accurate, consistent, trustworthy, unbiased. The data should also be current and the reference cited. The link to the dataset is here- [link](https://divvy-tripdata.s3.amazonaws.com/index.html).

This data is reliable, original, comprehensive and current as it is made publicly avaialble by Lyft Bikes and Scooters with the permission of the City of Chicago. Personally identifiable information such as credit card numbers has been removed because of data-privacy issues.

# 3. Process
The data is organized month by month from June 2020 to May 2021. 
The data contains information on the type of bicycle being used, at what time did the ride start and at what time did it end, latitude, longitude of the starting and ending location. Also has the whether the user is a casual rider or an annual member,

The data integrity is not satisfied as it has missing values, in some cases "started_at" time was later than "ended_at" although it may be accurate, consistent, trustworthy. 

I used pyhton for processing and cleaning the data.

1. Merged the 12 datasets togethers
2. Looked into misisng values. The columns that did have missing values, I did not require those for my analysis. That is why did not delete those rows with misisng values. 
3. Checked for duplicate entries. There were no duplicate entries.
4. Looked into the info() of teh dataset. The started_ata nd ened_at columsn were not in the correct format. they were strings and no datetime. Used pandas to_datetime() method to convert those to datetime.
5. Extracted "day of the week" and "month" from datetime
6. Noticed that in some cases "started_at" was at a later time than "ended_at". Swapped the entries so that "started _at" and "ended_at" can be swtiched to reflect lower "started_at" and higher "ended_at" time.

# 4. Analysis / Share
I did analysis on -
1. the percentage of casual and member riders in the entire dataset
![1  Total Bike Hires Per Rider category](https://user-images.githubusercontent.com/43137227/166157814-777c0507-eacb-46f3-8ef0-e12411dabe0d.PNG)

2. Total bike hires per month

![2  Total Bike Hires per Month](https://user-images.githubusercontent.com/43137227/166157948-e883ebcc-f706-4c73-8cd2-02476c714548.PNG)


3. Total Bike Hires per Day Of the Week

![3  Total Bike Hires per Day of the Week](https://user-images.githubusercontent.com/43137227/166158063-ee9613f4-e459-4ada-b82d-9072b57542c5.PNG)


4. Total Bike Hires per Rider Category per Day

![4  Total Bike Hires Per Rider Category Per Day](https://user-images.githubusercontent.com/43137227/166158151-5e9cfcab-be7f-4c2f-98c5-df06e6118ca3.PNG)


5. Average Ride Length Per Category Per Day

![5  Average Ride Length Per Category Per Day](https://user-images.githubusercontent.com/43137227/166158257-1f3cc840-29de-4b3f-afdb-dedfebf479c0.PNG)

6. Average Ride Length Per Month For Each category

![6  Average Ride Length Per Month For Each category](https://user-images.githubusercontent.com/43137227/166158400-755074ea-56f5-4b7e-89fe-9214e91594b8.PNG)




