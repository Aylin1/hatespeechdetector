Proposed Plan for Training an NLP Model to Classify Hate Speech Tweets

1) Get Twitter API
Sign up for the Twitter Developer Platform and obtain the API credentials. (https://developer.twitter.com/en/docs/developer-portal/overview) 
Check compliance with Twitter API usage policies (it seems there is no problem).

2) Collect Tweets
Select Topic:
Choose a specific topic (Palestine/Israel) to collect tweets about.
Tweet Extraction:
Use the Twitter API to extract approximately 150 tweets related to the chosen topic.
Polo will share the script to introduce the credentials, make the query and store in DataFrame (using “twitpy” library).

3) Define Hate-Speech
Hate-Speech Definition:
Clearly define what you consider as hate-speech. This might include offensive language, discrimination, threats, etc. In this case would be great if we get examples of “WHAT IS” and “WHAT IS NOT” hate-speech to be in the same page. Ideas for human-training:
Templates
Examples of WHAT IS and WHAT IS NOT
Manual Analysis:
Conduct a manual analysis of some tweets to have a clear understanding of what constitutes hate speech and what doesn't (50 twits each).

4) Label Tweets
Create Google Sheet:
Create a shared Google Sheet.
Define columns: "Twit_id," "message," "class," and any other relevant information.
Manual Classification:
Manually classify tweets as "TRUE" (if hate speech) or "FALSE" (if not hate speech).
Share the classification task, assigning different individuals to classify 1000 tweets each.

5) Structure Baseline Data
Baseline Data:
Ensure each tweet has a unique identifier ("Twit_id").
Include the "message" column with the tweet content.
Add the "class" column for classification (TRUE/FALSE).
You may include other relevant columns such as the tweet date, user, etc.
Is important to block and not modify text over message.

6) Train the Model (Using CRISP DM Logic)
Text Preprocessing: Clean and preprocess the text of tweets.
Data Splitting: Split the dataset into training and testing sets (80/20?).
Model Selection: Choose a suitable NLP model for the text classification task.
Model Training: Train the model using the labeled dataset.
Model Evaluation: Evaluate the model's performance using the test set.
Fine-Tuning and Improvement: Make adjustments to the model as necessary to improve its performance.
Document the entire process and classification criteria for future reference.
