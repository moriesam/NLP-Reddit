
## Project 3: Web APIs & NLP


### Executive Summary 

#### Technical Objectives: 

The purpose of this project is to utilize the Natural Language Processing (NLP) skills to collect posts from selected subreddits and then train a classifier to verify which subreddit a given post came from.

#### Data Science Process and Solution 

##### Selected subreddits used for this process are:

- r/globalwarming (https://www.reddit.com/r/climateskeptics/)
- r/Climateskeptica (https://www.reddit.com/r/GlobalWarming/)

The task here is to develop a model(decision making engine) that predicts post content on social news media (reddit) and then guides through making better decisions for climate change awareness. The model should also provide key insights for:

- which subreddit leverages engagement <br>
- key words to increase “climate literacy” <br>
- attitude & behavior towards related trends among members <br>


#### Data cleaning and preprocessing: 

The process included the following steps: 
 - Data pull from reddit and conversion to json
 - Removing data noise (removed url, punctuations, only kept a-z english letters)
 - Sentiment Analysis
 - Classifying content (0,1 classes)
 - Tokenizing, Lemmatizing, Vectorizing, setting Stop-words 
 - Tuning model, evaluation and selection

#### Tuned Models

- Random Forest 
- Logistic Regression 
- Gradient Boost 
- Voting Classifier 

In these models, text and related sentiment(the emotional tone  that determines if the topics used are positive, negative, or neutral context) are used as independant variables  to predict subreddit topic(target).<br>

#### Conclusion and Recommendations

- Logistic regression with 83.4% accuracy is the recommended model.<br>
- Even though the test score (83.4%) vs train score (90.7%) indicates 'overfitting', yet the model achieves a better performance compare to the baseline(~50%). <br>
**Next steps:**
- Fine-tune the model by optimizing parameters and set it up as our decision making engine<br>
- Set up a real-time dashboard for advanced analytics and tracking KPIs<br>
- Build an effective social media and content strategy plan based on our key findings 



