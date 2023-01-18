# Data-Wrangling-Project

Project: Wrangling and Analyze Data (WeRateDogs)

In this project, I performed the below wrangling processes to make the data clean and ready for analysis.

<ul>
<li><a href="#gathering">Data Gathering</a></li>
<li><a href="#assessing">Assessing Data</a></li>
<li><a href="#cleaning">Cleaning Data</a></li>
<li><a href="#analyzing">Analyzing and Visualizing Data</a></li>
</ul>


### Quality issues

* **twitter**

1. According to one of the project's requirements, we only want original ratings (no retweets) that have images. The retweeted tweets can be seen in columns like 'retweeted_status_id', 'retweeted_status_user_id', and 'retweeted_status_timestamp'.

2. Timestamp is an object instead of a datetime

3. In the name column, many entries contain invalid dog names such as none, a, quite, such, etc.

4. There are several duplicates in the expanded_url column.

5. For the dog styles (puppo, doggo, floofer, and pupper columns), missing values are represented as 'None' instead of 'NaN'.

6. There are inconsistencies in the name column with some dog names starting with capital letters while some starts with small letters.

7. Extract content from source column.

8. Cleaning rating_numerator and rating_denominator.

* **image**

9. There are duplicated entries with the same **jpg_url** but different tweet_id column.

10. There are inconsistencies in the columns like **p1, p2, p3** with some dog names starting with capital letters while some starts with small letters.

* **tweet**

11. create_date is an object instead of a datetime.

* General

12. tweet_id column in all the tables is stored as an int instead of a string.

### Tidiness issues

* **twitter**

1. Dog stages (doggo, floofer, pupper, and puppo) are in different columns and some dogs have more than one style:
    * tweet_id = 854010172552949000 (doggo and floofer)
    * tweet_id = 855851453814013000 (doggo and puppo) etc.

2. Merge the three datasets into one file.

### Insights:
1. What are the 3 most common dog names?

2. What is the most common dog style?

3. What has been the distribution of tweets over the years?

4. What is the most popular source of tweets?

5. What is the correlation between retweet_count and favorite_count?

6. What dog_style have the highest average retweet_count?

7. What dog_style have the highest average favorite_count?
