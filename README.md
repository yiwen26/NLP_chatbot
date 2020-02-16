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

## repo structure

```
│  .gitignore
│  config.py               #模型配置参数
│  corpus.pth              #已经过处理的数据集
│  dataload.py             #dataloader
│  datapreprocess.py       #数据预处理
│  LICENSE
│  main.py               
│  model.py       
│  README.md
│  requirements.txt
│  train_eval.py            #训练和验证,测试
│  
├─checkpoints              
│      chatbot_0509_1437   #已经训练好的模型
│      
├─clean_chat_corpus
│      qingyun.tsv         #语料库
│      
├─QA_data
│      QA.db               #知识库
│      QA_test.py          #使用知识库时调用
│      stop_words.txt      #停用词
│      __init__.py
│      
└─utils
        beamsearch.py      #to do 未完工
        greedysearch.py    #贪婪搜索，用于测试
        __init__.py
```

## Approach

#### QA System

- BiLSTM + attention


#### General Chatbot
- Seq2Seq
- Encoder: BiRNN
- Decoder: attention + biRNN

