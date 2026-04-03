# Experiment No: 15  
# Title: Preprocessing Techniques for Text Data and NLP Techniques on Text Data  

## Aim  
To study various preprocessing techniques and Natural Language Processing (NLP) methods used for analyzing text data.

---------------------------------------------------------------------

## Tools / Software Required  

• Python 3.x  
• Google Colab or Jupyter Notebook  
• Python Libraries:  
  o NLTK (Natural Language Toolkit)  
  o Pandas  
  o NumPy  

---------------------------------------------------------------------

## Theory  

### 1. Text Data  

Text data is a type of unstructured data that contains information in the form of words, sentences, or complete documents. Common examples of text data include emails, social media messages, product reviews, news articles, and chat messages.

Before performing analysis or applying machine learning algorithms, text data must be cleaned and prepared properly. This preparation process is known as text preprocessing.

---------------------------------------------------------------------

### 2. Preprocessing Techniques for Text Data  

Text preprocessing is the method of cleaning and converting raw text into a structured form so that computers can understand and analyze it effectively.

#### 1. Text Cleaning  

Text cleaning is used to remove unwanted elements from text such as punctuation marks, special characters, extra spaces, and unnecessary symbols. Removing these elements makes the text simpler, clearer, and easier to process.

--------------------------------------------------

#### 2. Lowercasing  

Lowercasing converts all uppercase letters into lowercase letters. This ensures that words with the same meaning but different letter cases are treated equally.

Example:  
Data Science → data science  

This reduces duplication and improves accuracy during analysis.

--------------------------------------------------

### 3. Tokenization  

Tokenization is the process of breaking text into smaller parts known as tokens. These tokens can be words, sentences, or characters.

Example:  
Sentence:  
"Natural language processing is useful"  

Tokens:  
Natural, language, processing, is, useful  

Tokenization makes it easier to analyze each word separately.

--------------------------------------------------

### 4. Stop Word Removal  

Stop words are frequently used words that do not carry significant meaning in text analysis.

Examples include:  
• is  
• the  
• and  
• in  
• of  

Removing stop words reduces unnecessary data and helps improve the efficiency of processing.

--------------------------------------------------

### 5. Stemming  

Stemming is the process of reducing words to their root form by removing suffixes.

Examples:

Word        Stem  
playing     play  
running     run  
studies     studi  

Stemming makes words shorter but sometimes produces words that are not found in dictionaries.

--------------------------------------------------

### 6. Lemmatization  

Lemmatization converts words into their base or dictionary form, known as a lemma. Unlike stemming, it considers grammar and meaning, making it more accurate.

Examples:

Word        Lemma  
running     run  
better      good  
studies     study  

Lemmatization produces meaningful root words.

---------------------------------------------------------------------

### 3. NLP Techniques on Text Data  

Natural Language Processing (NLP) is a branch of Artificial Intelligence that allows computers to understand, interpret, and analyze human language.

#### 1. Tokenization  

In NLP, tokenization is used to divide sentences into smaller parts such as words or phrases so that the system can analyze each component properly.

--------------------------------------------------

#### 2. Part-of-Speech (POS) Tagging  

POS tagging is used to identify the grammatical role of each word in a sentence. It assigns tags such as noun, verb, adjective, or adverb.

Example:

Sentence:  
"Python is powerful"  

Word        POS  
Python      Noun  
is          Verb  
powerful    Adjective  

This helps computers understand sentence structure.

--------------------------------------------------

#### 3. Named Entity Recognition (NER)  

Named Entity Recognition identifies important elements in text such as names of people, locations, organizations, and dates.

Example:

Sentence:  
"Elon Musk founded SpaceX."  

Entities identified:  
• Elon Musk → Person  
• SpaceX → Organization  

NER helps extract meaningful information from text.

--------------------------------------------------

#### 4. Sentiment Analysis  

Sentiment analysis is used to determine the opinion or emotion expressed in text. It identifies whether the text shows a positive, negative, or neutral feeling.

Example:  
Review: "This phone is excellent."  
Sentiment: Positive  

This technique is widely used to analyze customer feedback.

--------------------------------------------------

#### 5. Text Vectorization  

Text vectorization converts text data into numerical form so that machines can process it.

Common techniques include:

• Bag of Words (BoW)  
This method counts how many times each word appears in a document.

• TF-IDF (Term Frequency–Inverse Document Frequency)  
This method measures how important a word is in a document compared to other documents.

These methods represent text as numbers that can be used in machine learning models.

---------------------------------------------------------------------

## Applications of NLP  

NLP techniques are widely used in many real-world applications such as:

• Chatbots and virtual assistants  
• Language translation systems  
• Spam email filtering  
• Sentiment analysis of reviews  
• Search engines  
• Recommendation systems  

---------------------------------------------------------------------

## Conclusion  

Thus, preprocessing techniques and NLP methods used for analyzing text data were studied successfully. These techniques help clean text, extract useful information, and prepare text data for further analysis and machine learning tasks.
