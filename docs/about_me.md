## Research Interests:
I am interested in LLMs, RAG, Information Retrieval, Chatbots and Machine Translation.

## Projects:
* **bn-hi-MT-improvement-using-llm:**
  
  This project tries to explore two things:
  1. Check the English concept state in the middle layers of a llm using logit lens.
  2. If the MT for Bengali to Hindi using a open source LLM (in this case Mistral-7b-bnb-4bit quantized model) can be improved by     
  finetunig by using the parallel text.

  Project link: [bn-hi-MT-improvement-using-llm](https://github.com/arafat04/bn-hi-MT-improvement-using-llm).
  
  Project Report: [bn-hi-MT-improvement-using-llm report](https://drive.google.com/file/d/1qSiAulk-EULMIEEHllOYiMaHOfP0myE8/view?usp=sharing).

* **travelbot - a chatbot to find hotels and flights:**
  
  This is a probabilistic and rule based chatbot. The Natural Language Understanding(NLU), policy are rule-based, Natural Language 
  Generation(NLG) is template-based, and probabilistic dialogue/belief state tracker to work with NLU. The job of the belief state 
  tracker is to help the chatbot to use probability to find most probable slot values if the user wrote the utterance in not an 
  usual way i.e. spelling mistake. This work like this:

  The update rule for a slot, say food, We take all mentions of food in the current NLU, with their probabilities. 
  Say we got Chinese with a probability of 0.7 and Italian with a probability of 0.2. This means None (or null) has a probability of 0.1. 
  We use the probability of None to multiply current values with it (e.g. if the distribution was {'Chinese': 0.2, None: 0.8}, it should 
  be changed to {'Chinese': 0.02, None: 0.08}. Now addition of the non-null values with their respective probabilities from the NLU. This 
  should result in {'Chinese': 0.72, 'Italian': 0.2, None: 0.08}.. Then the rule-based policy    that uses the current NLU intent (or 
  intents, coming from our NLU) and the dialogue state (coming from our tracker) to produce system action dialogue acts. For example:

  ```
  U: Hello, I need a cheap restaurant
  S: hello()&confirm(price=cheap)&request(area)
  Here, U: user utterance, S: system utterance
  ```
 
  Based on the dialogue acts, the template is used for generating natural language.

  Video demo of the project: [travelbot demo](https://youtu.be/lYnPE4exrls).
  
* **Identifying-Offensive-Language-in-Socail-media-using-NLP:**
  
  In this project, I used various NLP techniques such as tokenization, POS tagging, word representation using TF-IDF and word embedding     using GloVe and Finally evaluated the performance using Logistic Regression and Naive Bayes and using a Recurrent Neural Network.
  
  Project report: [ResearchGate](http://dx.doi.org/10.13140/RG.2.2.25084.21121). | Project github Link:  [Identifying-Offensive-Language-in-Socail-media-using-NLP](https://github.com/arafat04/Identifying-Offensive-Language-in-Socail-media-using-NLP).

* **Markov Chain Analysis with R:**

  R Separate weather and stock price datasets were analyzed, and a Markov
  chain model was developed in R to predict weather and stock price trends.

  Project page: [Markov chain analysis with R](https://arafat04.github.io/Markov-Chain-Analysis/).

  [Erasmus Mundus LCT](https://lct-master.org/) | [UFAL, Charles University](https://ufal.mff.cuni.cz/home-page) | [IDMC, University of 
  Lorraine](https://idmc.univ-lorraine.fr/courses/master-degree-2-nlp/)

  
