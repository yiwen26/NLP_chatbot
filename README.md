# MH6812_Advanced NLP with Deep Learning
## Insurance Question & Answer Chatbot

## Background
A chatbot is a piece of software that conducts a conversation via auditory or textual methods. Chatbots are typically used in dialog systems for various practical purposes including customer service or information acquisition.   
Chatbot framework can be divided into four areas according to two dimensions, responses and conversations. Responses include retrieval-based and generative-based. Conversations include open domain and close domain.

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
This kind of chatbot is used in open field chat scenario, just as chat between friends without the limitation of topics or contents.    
General chatbots are usually based on seq2seq architecture, using models to generate answers automatically and optimizing them by combining technologies such as Attention.  
## Motivations
- Market: People regard insurance as necessity. Insurance market is expanding.
- Customer: Not every customer or potential customer is assigned with a customer manager. Chatbot will help solve their problem.
- Company: Chatbot will free manpower and increase working efficiency.

