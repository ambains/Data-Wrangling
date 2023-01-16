# Data-Wrangling-in-Jupyter-Notebook-with-Pandas

The process of Data Analysis typically involves three steps: gathering, assessing, and cleaning data. 
This project applied these steps to a Twitter account data, specifically focusing on the account "weratedogs" 
and their unique rating system, where the rating numerator is not bounded, but the rating denominator must remain 10.

The first step in Data Analysis is collecting data. In this project, data was collected from three sources: a CSV file,
a URL, and an API. The CSV file, named "twitter-archive-enhanced.csv," was provided by Udacity for download and import 
into a Jupyter notebook. The second source was a URL, where the dataset was stored and required the use of the "requests" 
library in Python to retrieve the data and store it in the "twitter-archive-enhanced.csv" file. The third source was Twitter's 
API, which was accessed using the "tweepy" library, provided that the person has a Twitter account and is approved to collect data from the API.

After collecting the data, the next step is assessing the data. This was done using a combination of Python built-in methods 
such as "df.info()," "df.describe()," "df.head()," "df.sample()," "df.value_counts()," "df.isnull()," and "df.duplicated()." 
Additionally, visual assessment was done using "df.head()" and "df.sample()," to identify issues with the quality and tidiness of the data.

After identifying eight quality issues and two tidiness issues, the next step is to clean the data. It is best practice to 
address completeness and tidiness issues first, as this ensures that the dataframe is complete and well-structured for analysis. 
However, there may be instances where data cannot be completed, and reasons for incompleteness include user not entering information 
or lack of activity on certain attributes of the dataframe. In this project, two tweet_ids were missing from the tweets_list_df, 
but were not present in the "tweet-json.txt" file, indicating that these tweet_ids did not have retweets or favorites.

After resolving the identified issues, the cleaned master dataframe was saved as a CSV file in Jupyter notebook for further 
exploratory data analysis.
