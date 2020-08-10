# Marketing Analysis
![https://www.freepik.com/free-photos-vectors/mail](https://image.freepik.com/free-vector/mailbox-concept-illustration_23-2148277017.jpg)
#### From: https://www.freepik.com/free-photos-vectors/mail
How to increase the e-mail open rate?

## Background
The aim of this project is to build a model that can predict whether a user opens the emails or not.

Sending emails is one of the marketing channels to reach out to our users. Being able to predict whether a user opens an email allows a company to forecast and evaluate the performance of future marketing campaigns before launch. This is because when a user opens an email, the probability of the user knowing the campaign increases and this in turn increases the probability of the user making a checkout during the campaign period. Therefore, with the predicted open rates, a company can better develop, strategize and implement future marketing campaigns.

## Datasets
- User-specific information
- Email nature
- Users’ engagement on the platform
- User’s reaction to the email, including whether users opened the email

### File description
- train.csv: the training set
- test.csv: the test set
- users.csv: user's information
- sample_submission_0_1.csv: a sample submission file in the correct format
### Data fields
#### Train/Test.csv
- country_code - an anonymous id unique to a given user comments
- grass_date: The date when the email was sent.
- user_id: the unique identifier of each user
- subject_line_length: the number of characters in the subject of the email
- last_open_day: How many days ago was the last time the user opened an email
- last_login_day: How many days ago the user last logged in its Shopee account
- last_checkout_day: How many days ago the user last purchased on Shopee
- open_count_last_[10/30/60]_days: the total number of email opens in the last N days.
- login_count_last_[10/30/60]_days: the total number of user logins in the last N days.
- checkout_count_last_[10/30/60]_days: the total number of checkouts (=purchases) by the user in the last N days.
- open_flag: the target variable. Whether or not the email was opened.
- row_id:
#### users.csv (empty values are simply unknown)
- user_id: the unique identifier of each user
- attr_[1/2/3]: general user attributes. Attr_1 and attr_2 are boolean, attrib_3 is categorical (can be integer [0,1,2,3,4])
- age: The user's reported age.
- domain: The user's top-level email domain. Less common domains are bundled together under the label 'other'.
#### sample_submission_0_1.csv: 
A valid submission file.
### Train/Test.csv
| country_code | grass_date | user_id | subject_line_length | last_open_day | last_login_day | ..... |
| :-: | :-: | :-: | :-: | :-: | :-: | :-: | 
| 4 | 2019-07-16 00:00:00+08:00 | 43 | 44 | 19 | 6 | ..... |
| 4 | 2019-07-16 00:00:00+08:00 | 102 | 44 | 9 | 4 | ..... |
| 6 | 2019-07-16 00:00:00+08:00 | 177 | 49 | 14 | 5 | ..... |
| 1 | 2019-07-16 00:00:00+08:00 | 184 | 49 | 49 | 9 | ..... |
|..... | ..... | ..... | ..... | ..... | ..... | ..... |
### users.csv
| user_id | attr_1 | attr_2 | attr_3 | age | domain |
| :-: | :-: | :-: | :-: | :-: | :-: | 
| 0 |  | 1.0 | 0.0 |  | @gmail.com |
| 1 | 1.0 | 1.0 | 2.0 | 50.0 | @gmail.com |
| 2 |  | 1.0 | 0.0 |  | other |
| 3 |  | 1.0 | 0.0 |  | @gmail.com |
| 4 | 1.0 | 1.0 | 2.0 | 33.0 | @gmail.com |
| ..... | ..... | ..... | ..... | ..... | ..... |
### sample_submission_0_1.csv
| row_id | open_flag |
| :-: | :-: | 
| 0 | 1 |
| 1 | 1 |
| 2 | 1 |
| 3 | 1 |
| 4 | 1 |
| ..... | ..... |
