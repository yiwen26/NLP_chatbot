# NLP_banking_chatbot

## Background
A chatbot is a piece of software that conducts a conversation via auditory or textual methods. Such programs are often designed to convincingly simulate how a human would behave as a conversational partner. Chatbots are typically used in dialog systems for various practical purposes including customer service or information acquisition. Some chatbots use sophisticated natural language processing systems, but many simpler ones scan for keywords within the input, then pull a reply with the most matching keywords, or the most similar wording pattern, from a database.

## Type of chatbot
There are three types of chatbot: QA, Dialogue System, General chatbot.
#### QA
This type is based on questions from users. Answers given by the bot are not required to form dialogues. This kind of chatbot is usually used for intelligent searching and smart home. QA does not have to fulfill any business target. What the chatbot does is only to give matched answers to users’ questions. QA usually focuses on one specific area and provides services to customers.\<br>
Before building the QA system, a large dataset of FAQ is required. There are three methods to train the models.\<br>
- Calculate the similarity of queries from users and questions in dataset. Then map the highest similarity question with the answer.\<br>
- Calculate the relevance between queries and answers. Then map the highest relevance answers to the questions.\<br>
- The combination of two above.\<br>
#### Dialogue System
Dialogue system usually focuses on missions. The chatbot needs to interact with users, even in multiple rounds. After recognizing the requirement of users, the chatbot has to finish the business task. For example, when the user asks the weather chatbot about the weather, this chatbot will judge if it can get the real-time information of weather. If it cannot reach the weather information, it will ask the user and then get the data from some websties. The application scenarios of the dialogue system are very rich, such as customer service robot, sales robot and so on.\<br>
Dialogue system contains NLU, DM and NLG. NLU is used to understand the input of users, including intention identification and entity identification. DM is used to manage the dialogue, including slot management, behavior decision, data acquisition. NLG is used to generate answers to users’ questions.\<br>
#### General Chatbot
This kind of chatbot is used in open field chat scenario, just as chat between friends without the limitation of topics or contents. This kind of chatbot is mainly used as personal assistant, entertainment and other scenes, typical representatives such as Microsoft ice, apple Siri and so on.\<br>
It is very difficult to develop this general chatbot. Huge datasets and high quality algorithms are required.\<br>
General chatbots are usually based on seq2seq architecture, using models to generate answers automatically and optimizing them by combining technologies such as Attention. Currently, Attention and other techniques are introduced to achieve better coding for users. In order to realize the model's ability to understand the user's previous and subsequent input, user history encoding is introduced. This approach is based entirely on data and has the advantage of being flexible and not requiring complex dialogue management. The disadvantage is that the controllability is not strong. The generated answers are often short, and many meaningless answers are returned. Also, a large amount of training data is required.

