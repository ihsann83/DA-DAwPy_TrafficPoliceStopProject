# DA-DAwPy_TrafficPoliceStopProject_01

# Examining the dataset

I analyzed a dataset of traffic stops in Rhode Island that was collected by the Stanford Open Policing Project.

Before beginning the analysis, I became familiar with the dataset;

I read the dataset into pandas, examined the first few rows, and then counted the number of missing values. I dropped the 'county_name' column because it only contains missing values, and I dropped the 'state column' because all of the traffic stops took place in one state (Rhode Island). Thus, I dropped those columns, because they contain no useful information.The 'is_arrested' column currently has the object data type. I changed the data type to bool, which is the most suitable type for a column containing True and False values. So, I use mathematical operations on the is_arrested column that would not be possible otherwise. I combined 'stop_date' and 'stop_time' into a single column, and then converted it to datetime format. So, this will enable convenient date-based attributes that I will use later. I set the 'stop_datetime; column as the DataFrame's index. By replacing the default index with a DatetimeIndex, I will make it easier to analyze the dataset by date and time.

Then, I made analysis to explore the relationship between gender and policing;

I examined the violations committed by all drivers to get a baseline understanding of the data, before comparing the violations being committed by each gender. I counted the unique values in the 'violation' column. In order to understand whether male and female drivers tend to commit different types of traffic violations, You'll first create a DataFrame for each gender, and then analyze the violations in each DataFrame separately.






