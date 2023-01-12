# Data-Wrangling-Project

Project: Investigate the TMDb Dataset

In this project, I performed the below wrangling processes to make the data clean and ready for analysis.

<li><a href="#gathering">Data Gathering</a></li>
<li><a href="#asssessing">Data Assessing</a></li>
<li><a href="#cleaning">Data Cleaning</a></li>

### Quality issues

* tweet

1. Timestamp is an object instead of a datetime

2. In the name column, many entries contain invalid dog names such as none, a, quite, such, etc. 

3. There are several duplicates in the expanded_url column.

4. Missing values are represented as 'None' instead of 'NaN'.

5. There are inconsistencies in the name column with some dog names starting with capital letters while some starts with small letters.

6. Some dogs have more than one style:
    * tweet_id = 854010172552949000 (doggo and floofer)
    * tweet_id = 855851453814013000 (doggo and puppo) etc.

* image

7. There are duplicated entries with different tweet_id column but having the same entry in the other columns.

* tweet

8. create_date is an object instead of a datetime.

* General

9. tweet_id column in all the tables is stored as an int instead of a string.

### Tidiness issues

* twitter

1. Dog stages (doggo, floofer, pupper, and puppo) are in different columns. 

2. Only 'original tweets' are of interest in this analysis. The retweeted tweets can be seen in columns like 'retweeted_status_id', 'retweeted_status_user_id', and 'retweeted_status_timestamp'.
