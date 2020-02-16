# MH6812_Advanced NLP with Deep Learning
## Insurance Question & Answer Chatbot 

We built a Chatbot with both the functions of general chat and Q&A (insurance questions). 
![chatbot](https://github.com/yiwen26/NLP_chatbot/blob/master/graph/%E5%9B%BE%E7%89%871.gif)

### Background

Chatbot framework can be divided into four areas according to two dimensions, responses and conversations. Responses include retrieval-based and generative-based. Conversations include open domain and close domain.


> Type of chatbot

There are three types of chatbot: QA, Dialogue System, General chatbot. In our project, we combined the QA and general chat into our chatbot.

>- QA

This type is based on questions from users. Answers given by the bot are not required to form dialogues. QA does not have to fulfill any business target.    
There are three methods to train the models.    

    - Calculate the similarity of queries from users and questions in dataset. Then map the highest similarity question with the answer.    

    - Calculate the relevance between queries and answers. Then map the highest relevance answers to the questions. *This is what we used in the project*

    - The combination of two above.  

>- General Chatbot

This kind of chatbot is used in open field chat scenario, just as chat between friends without the limitation of topics or contents.    
General chatbots are usually based on seq2seq architecture, using models to generate answers automatically and optimizing them by combining technologies such as Attention.  

### Motivations

- Market: People regard insurance as necessity. Insurance market is expanding.

- Customer: Not every customer or potential customer is assigned with a customer manager. Chatbot will help solve their problem.

- Company: Chatbot will free manpower and increase working efficiency.

## Repo Structure

```
│  LICENSE   
│  README.md
├─QA system              
│       ├─data                                  # raw text corpus
│       │   answers.label.token_idx
|       |   question.dev.label.token_idx.pool
|       |   question.test1.label.token_idx.pool
|       |   question.test2.label.token_idx.pool
|       |   question.train.token_idx.label
|       |   vocabulary
|       ├─model                                 # trained model save to dir
|       |   demo.model                          # demo_model
|       | README.md
|       | main.py                         
|       | model.py                              # model building
|       └─ preprocess.py                         # data preprocess      
├─general chatbot
│       ├─Data Preprocessing
|       |   data_preprocess.py
|       |   format_twitter.txt                   # twitter data after preprocessing
|       |   formatted_movie_lines.txt            # movie data after preprocessing
|       ├─data                                   # raw data
|       |   movie_characters_metadata.txt
|       |   movie_conversations.txt
|       |   movie_titles_metadata.txt
|       |   raw_script_urls.txt
|       |   twitter_chat.txt
│       ├─save                                   # trained model save dir
|       | config.py
|       | evaluate.py
|       | load.py
|       | main.py
|       | model.py
|       | pairlist.py
|       | train.py
```

## Approach

#### QA System

- BiLSTM + attention


#### General Chatbot
- Seq2Seq
- Encoder: BiRNN
- Decoder: attention + biRNN

