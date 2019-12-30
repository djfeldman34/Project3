# Text Sentiment Analysis
Utilizing Zipf’s Law, our team is looking to analyze the sentiment of text structure in a given sentence.  A Zipf distribution is a repeatable and naturally occurring layout of data that shows up in word prevalence.  Our goal is to analyze the structure of Yelp reviews and Datafiniti Hotel Reviews to determine the sentiments of users as they write reviews while incorporating Zipf’s law to improve efficiency by removing non-descriptive words. 
In order for our team to make an accurate analysis of the data being utilized, we can expect to use a minimum viable word count to make an accurate prediction. The team will create a mechanism for user input to get the appropriate sentiment analysis. 
The team will present this through a web app using Machine Learning, Flask, MongoDB, JavaScript, and HTML/CSS. 
## Team Members
Abdurrahman Darvesh, DJ (David) Feldman, and Zack Feldman
## Hypothesis
Given a sufficiently large set of text, we can determine the positive or negative sentiment of the author.
## Null Hypothesis
Given a sufficiently large set of text, we are unable to determine the sentiment of the author.
## Goals/Intended Outcomes
1.  Prove the existence of Zipf’s law in random sets of text
2.  Use Machine Learning to build a model to predict the sentiment of a given set of text
3.  Determine the critical word count required to get an accurate sentiment.
## Data Sets Used
1.  Database of positive/negative reviews
2.  Database of movie/business reviews
3.  Flask App to access database, and JS/HTML representation
## Milestones
### I.  Mung Data
Getting datasets through Kaggle. Formatting datasets so that they can be saved as .bson format. 
### II.  Setup Database
Setting up multiple collections through PyMongo. Broke the dataset up by review types such as hotel review and business reviews through Yelp and Datafiniti. Breaking it down by a Review ID, User ID, Business ID, Stars, useful or helpful Upvotes by other users, funny count determined by other users, cool factor determined by other users and then the text of the actual review itself
### III.  Build Machine Learning Models
Use the data sets and SKLEARN to train a model that will be able to determine which sentences lend themselves to positive or negative connotations.  We will use supervised learning by using the review text as the input and whether the review is high (i.e. 5 stars) or low (i.e. 1 star) as the goal.
### IV.  Build Front-End Application
Develop Flask App to access the data and visualizations.  User access to input where sentiment analysis can be used.  Create an interactive and fun experience that entices the user to explore our product.
## Constraints
Potential roadblocks our product could run into include:
<ul>
  <li>Fake reviews</li>
  <li>Sarcastic reviews</li>
  <li>Invalid reviews such as a typo or unfinished reviews</li>
  <li>Subtle underlying messages within a review</li>
  <li>The authenticity of a review</li>
</ul>

# Conclusions
After using several different models, we concluded that the best model for this type of task is a Neural Network model.  We were able to acheive a 79% accuracy rate with this model.  This result needs to be taken with a grain of salt because the data itself is skewed and not equally distributed (i.e. the dataset contains 72.7% positive reviews).  

The most important part of the functionality of the Neural Network model is the fact that it lowers the type I and type II errors more than any other of the models.

# Project Status
The functionality of the live application testing of input text is still under development.

We are still working on converting the visualizations into a useful market prediction tool.
