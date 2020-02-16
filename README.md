# MH6812_Advanced NLP with Deep Learning
## Insurance Question & Answer Chatbot

## Background
A chatbot is a piece of software that conducts a conversation via auditory or textual methods. Chatbots are typically used in dialog systems for various practical purposes including customer service or information acquisition.   

## Type of chatbot
There are three types of chatbot: QA, Dialogue System, General chatbot.  
#### QA
This type is based on questions from users. Answers given by the bot are not required to form dialogues. QA does not have to fulfill any business target.    
There are three methods to train the models.    
- Calculate the similarity of queries from users and questions in dataset. Then map the highest similarity question with the answer.    
- Calculate the relevance between queries and answers. Then map the highest relevance answers to the questions. This is what we used in the project.     
- The combination of two above.  
#### Dialogue System
Dialogue system usually focuses on missions. The chatbot needs to interact with users, even in multiple rounds. After recognizing the requirement of users, the chatbot has to finish the business task.   
Dialogue system contains NLU, DM and NLG.
#### General Chatbot
This kind of chatbot is used in open field chat scenario, just as chat between friends without the limitation of topics or contents. This kind of chatbot is mainly used as personal assistant, entertainment and other scenes, typical representatives such as Microsoft ice, apple Siri and so on.  
It is very difficult to develop this general chatbot. Huge datasets and high quality algorithms are required.  
General chatbots are usually based on seq2seq architecture, using models to generate answers automatically and optimizing them by combining technologies such as Attention. Currently, Attention and other techniques are introduced to achieve better coding for users. In order to realize the model's ability to understand the user's previous and subsequent input, user history encoding is introduced. This approach is based entirely on data and has the advantage of being flexible and not requiring complex dialogue management. The disadvantage is that the controllability is not strong. The generated answers are often short, and many meaningless answers are returned. Also, a large amount of training data is required.

