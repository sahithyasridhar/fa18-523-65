# Natural language text processing and Language generation :wave: :exclamation: fa18-523-67, fa18-523-65

| Sahithya Sridhar, Prajakta Patil
| sahsrid@iu.edu, patilpr@iu.edu
| Indiana University, Bloomington
| hid: fa18-523-67, fa18-523-65
| github: [:cloud:](https://github.com/cloudmesh-community/fa18-523-65/blob/master/paper/paper.md)
 
:o: not yet reviewd

:o: your paper was one of the paper that motivated us to send out a mail on reminding people to read the FAQ and do prope rmarkdown format using for example empty lines where they need to be. We hoped you would have read the FAQ and applied to your paper.

:o: also makrdoen requires a space after >

:o: please review rules on when to use would, will and is

## Introduction

> "The goal of NLP is to accomplish human-like language processing 
[@www-liddy1998nlp]".

Natural language processing (NLP) forms the link between machine language 
(binary code) to natural languages (which we humans speak). It borrows elements
from artificial intelligence, computer science and information engineering.
Success of NLP is highly dependent on how one can successfully program 
computers, to process, analyze and interpret huge amounts of natural language 
data. Key challenges/opportunities in this inter-disciplinary field involves 
speech recognition, language interpretation and generation of natural language
from a machine representation.With NLP, it is possible for computers to read 
text, hear speech, interpret it, measure sentiment and determine which parts 
are important [@www-sasnlp].

:o: this does not belong in an abstract 

NLP was initially called NLU (Natural language understanding). A natural
language understanding system will be used to paraphrase the input text,
will be able to translate text into another language, analyze the content of
the text and draw conclusions. As NLP still cannot draw inference from the text,
it is still dependent on NLU. One example of such difficulty is understanding
if a certain word in a sentence is a noun or a verb. For example, word ‘leave’
can be either a noun or a verb depending on context of sentence. 

## keywords
Natural language process :o: , Machine learning, Big Data, yelp data

:o: does not follow our sample

## Purpose of Natural language processing 

It is well known [:o: citation missing] that quite a bit information which exists out in our world is
very unstructured. The challenge would (:o: grammar) be to make a computer to understand this
and extract data from it. (:o grammar?) Take English language as an example. Humans have been
writing down things for thousands of years but computers can’t (:o: no contrations see our FAQ) yet truly
understand the language as we do. The trick is to break down the process of
understanding English into smaller chunks and understanding each smaller piece
separately [@www-sasnlp].

According to [@www-liddy1998nlp] Natural language processing has two distinct
focuses:

* *Language processing:* Produces a meaningful representation by analyzing the 
 language. This is similar to a machine reading the text.
* *Language generation:* language is produced from representation. This requires
 a planning capability. This is similar to a machine writing the text. 
 
The text is manipulated for abstractions and indexed for automatic knowledge
extraction. Producing text in a desirable format is one of the major research
areas in NLP. Structuring of large bodies of textual information to retrieve an
information is classified under the Natural language text processing
[@www-liddy1998nlp].

> "The central
task for natural language text processing systems is the translation of
potentially ambiguous natural language queries and texts into unambiguous
internal representations on which matching, and retrieval can take place"
[@www-liddy1998nlp].

## Levels of NLP

Past research concentrating on natural language text processing systems has been
reviewed by many [@www-haas1996nlp]. :o: yet there is only one refernce?
The various important terminologies of Natural Language Processing are: 

:o: incosistent use of empty lines results in that markdown can not format properly and consistently

 * *Phonology:* Refers to the understanding of sound of individual words and
    groups of words when spoken together in a sentence of sound. There are three 
    types of rules used here: 
    
 :o: indntation wrong
 
  > "
    * *phonetic rules:* for sounds within words; 
    * *phonemic rules:* for variations of pronunciation when words are spoken 
          together, and
    * *prosodic rules:* for fluctuation in stress and intonation
          across a sentence [@www-liddy1998nlp]."
     
* *Morphology:* Comprises of nature of words where the different parts of the
   words represent smallest units. A word can be broken down into its 
   constituent morphemes to understand the meaning [@www-liddy1998nlp].
   This involves understanding suffixes/prefixes attached to words, whether
   the word is singular or plural, root of words.
   
*	*Lexical:* Interprets the meaning of the sample word. Words that have only 
   one meanings is replaced by the semantic representation of a word. This 
   requires the word to have a simple or a complex lexicon [@www-liddy1998nlp].
*	*Syntactic:* Rectifies the grammatical mistakes in a sentence. The output 
   reveals a pattern that has a structural dependency between the words.
   Variours grammars are used which in turn affects the choice of the parser.
   As the order  of the words convey different meanings syntax conveys meanings
   in most languages [@www-liddy1998nlp].
   
*	*Semantic:* Determines the meaning of the word by looking at the interactions
   among word-level meanings in the sentence. Example of this would be trying to
   understand if word ‘honey’ is used as noun or adjective in given sentence.
   
*	*Discourse:* Focusses on properties of the text that convey meaning by making
   connections between component sentences. This helps understand what part of 
   story are certain set of sentences conveying.
  
  >"Discourse/text structure recognition determines the functions of sentences in
    the text, which, in turn, adds to the meaningful representation of the text"
    [@www-liddy1998nlp].
    
* *Pragmatic:* It is concerned with the firm use of the language. The main
   goal is the use of the context over the content of the text
   for understanding. This helps how to determine not so obvious additional
   meaning of words than what is captured in plain text of a sentence
   [@www-chaudhary2003nlp]. 
   
Current NLP system tends to implement those models that are used for 
processing the lower levels as they have been well researched and implemented
and also the applications do not require them to process at the higher levels
[@www-liddy1998nlp].

## Natural Language generation

According to [@www-khurana2017nlp]this part of NLP happens in four phases:
*	*Identifying the goal:* Meaning, defining if we want to generate language
   in form of written text or spoken words
   
*	*Evaluating the situation and planning to achieve the goal:* This involves
   identifying how said goal can be achieved by breaking it in individual tasks.
   
*	*Evaluate the available resources:* Depending on whether we want to generate
   written text or spoken words, we must evaluate if this can be achieved with 
   current communication devices. 
   
*	Execute the plans as text.

## Approaches to NLP:

According to [@www-liddy1998nlp] some approaches of NLP are as follows:

* *Symbolic Approach-* Performs deep analysis of linguistic phenomena based on 
   the human developed rules and lexicons. Logic or rule based systems and 
   semantic networks are good examples of symbolic approach.
   
   >"Symbolic approaches have been used for a few decades in a variety of research
   areas and applications such as information extraction, text categorization, 
   ambiguity resolution, and lexical acquisition [@www-liddy1998nlp]"
   
* *Statistical Approach-* Various mathematical techniques are used here. Observable 
   data is used mainly as evidence. Hidden Markov model is a widely used
   statistical approach. This is used in speech recognition, parsing, statistical
   grammar learning etc.
   
* *Connectionist-* Models are developed based on the linguistic phenomena. This 
   combines statistical model with other theories. 
   
Statistical Approach has been proven to work best on lower level of natural language
processing. Lower level of processing means analysis on level of parts of words, words
and sentences. Symbolic Approach works on both lower and higher level of processing.
Higher level of processing is analysis based on inferences from set of sentences and
understanding of whole text in a given document [@www-liddy1998nlp]. 

## Related Work

Significant research has been done on natural language processing since 1940s.
This has resulted in development of tools such as Sentiment Analyzer, Parts of
Speech Taggers, Emotion Detection, Semantic Role Labelling etc. Development of
such tools has allowed this technology to create real world applications such as 
Google search, Apple’s Siri, Amazon’s Alexa etc. Applications such as these has 
further increased interest in NLP as a useful research topic  [@www-liddy1998nlp].

Researchers working on NLP, building tools and systems which makes NLP what it
is today. Tools like Sentiment Analyzer, parts of speech, Emotion detection,
Semantic Role Labelling etc made NLP a good topic for research
[@www-khurana2017nlp].

* *Sentiment Analyzer:* Analyses the document for positive and negative words.
  It uses the sentiment lexicon and the sentiment pattern database to analyze the
  sentiments.

* *Parts of speech:* It can efficiently tag and classify words as nouns, adjectives,
  verbs etc. Parts of speech are assigned to tokenized data. Taggers are already 
  present for the  European languages, research is being done on making parts of 
  speech taggers for other languages like Arabic, Sanskrit [@www-tapaswi2012nlp], 
  Hindi [@www-ranjan2003nlp] etc.
  
* *Emotion Detection:* This is like sentiment analysis, but it works on social media
  platforms on mixing of two languages. It categorizes statements into six groups
  i.e. anger, disgust, fear, happiness, sadness and surprise based on emotions in 
  text [@www-khurana2017nlp].

* *Sematic Role Labelling:* SRL works by giving a semantic role to a sentence.
  Like assigning roles to words that are arguments of a verb in the sentence.
  This helps understand which words indicate action being done, which ones 
  indicate result of action and words that show who is doing the action etc 
  [@www-palmer2005nlp].

## Applications of NLP

Natural Language Processing can be applied into various areas like Machine
Translation, Email Spam detection, Information Extraction, Summarization,
Question Answering etc. According to [@www-khurana2017nlp] some more applications
of NLP are:

* *Machine Translation:* As the name suggests Machine translation is translating a
  phrase from one language to another with the help of engines like google
  translate. The major challenge in machine translation is keeping the meaning and
  the grammatical structure of the translated language intact.

* *Text categorization:* Splitting the large volume of data into several categories.
  Example spam filters. This usually works by either looking at email subject, content
  or sender blacklisted by receiver. It is also used to categorize communication so as
  to forward them to appropriate department when used in business setting. 

* *Spam Detection:* Various machine learning techniques like Rule Learning,
  Naïve Bayes, Memory based Learning, Support vector, Decision Trees,
  Maximum Entropy Model etc. are used to detect the spams. This is very similar to 
  text categorization.
  
*	*Chatbot:* A chatbot is a computer trying to mimic human like interaction/
   communication. We see many applications of these currently on different banking
   /ecommerce websites. Currently, computers are capable of handling simple question and 
   answering tasks. There is lot of research going on to make this even more capable
  
## Problems with natural language processing: linguistic variation and ambiguity 

There are certain problems is natural language processing that reduce the efficacy 
of textual information retrieval. linguistic variation and ambiguity are some of 
the problems in NLP. Linguistic variation is an issue when the same words or 
expressions are used to communicate the idea. Multiple interpretations is the 
main problem with Linguistic variation. Linguistic Variation provokes the 
omission of certain documents that are relevant and Ambiguity implies when a 
document has duplicate words or words that are not related [@www-mari2011nlp].
```
Example 1: A notebook was the present that the teacher gave him, when we were
present in the class.
```
Here the word "present" has different meanings both as an adjective and as a noun.
The word present plays different morph-syntactic depending on the situation,
causing ambiguity problems.
```
Example 2: He ate food on the car.
```
Ambiguity is produced here again, as this sentence can have several meanings 
like, he ate the food which was present in the car, or he ate food when he was 
driving the car.
```
Example 3: I went to the bank.
```
Here the bank could mean a place where save money and transactions are made or
a mound.

These examples show that automated process is not easy and that how complex the
language is. Statistical processing of NLP and specifically machine learning has
improved understanding of learning language by training on text corpus 
[@www-wikinlp].

## Natural Language processing in textual information retrieval

When the user gives a query, the following task are performed as a part of 
Natural Language processing's textual information retrieval
[@www-mari2011nlp]:

* Index is created for the descriptions of a document based on the NLP
techniques.

* When a query is given by a user the system analyses it and transforms it
such that it is similar to what is represented in the document.

* The description of each document is compared by the system with the query
given by the user, and those documents that have the description close to the 
users query to retrieved. There are different methods used to perform job of 
matching a query and document. Boolean method does this by trying to do exact 
match. Vector space model converts query and documents in vectors that can be 
stored as matrices. It then finds similarity by calculating cosine angle between 
query and document vector. Another method used to perform this is language model.
Language model tries to find probability of document generating a query. This model
depends on training the algorithm on large corpus of text data/documents.

* The results are shown in the order of the similarity. Google uses PageRank to rank
the documents in terms of similarity to query from user

## Statistical processing of natural language

> "This is a very simple focus based on the "bag of words." In this approach,
all words in a document are treated as its index terms. Moreover, each term is
assigned a weight in function of its importance, usually determined by its 
appearance frequency within the document. This way the word's order, structure,
meaning, etc., are not taken into consideration [@www-mari2011nlp]."

The document processing model involves document pre-processing and Parameterization.

* *Document pre-processing:* Prepares the documents by removing those elements that
are superfluous. There are three basic phases here:

   * Removing headers, tags etc. from the document which are not for indexing.
   *	Tokenization splits text into sentences and sentences into words
   * Standardizing  the text by checking for capitalized or non-capitalized
   letters, numerals, dates etc.Making all words lowercase helps treat words 
   such as ‘Hi’ and ‘HI’ same. 
   * Stemming the terms by reducing the words to the roots.This operation removes
   suffixes, prefixes etc.

* *Parameterization:* Assigns weights to the relevant terms present in the document.

:o: indentation wrong markdown is now confused

> "quantifying the document's characteristics
 [@www-mari2011nlp]."

One of the most used methods to estimate the importance of a term is the TFIDF
system (Term Frequency, Inverse Document Frequency).

> "It is designed to calculate the importance of a term relative to its appearance
frequency in a document, but as a function of the total appearance frequency for
all of the corpus' documents. That is, the fact that a term appears often in one
document is indicative that that term is representative of the content, but only
when that term does not appear frequently in all documents. If it appeared frequently
in all documents, it would not have any discriminatory value [@www-mari2011nlp]."

Two commonly used techniques in statistical processing are:

* *Detecting N-Grams:* This involves identifying compound words, proper nouns etc.,
to be able to process them as single words. This is done by determining the 
probability of the compound words like European union etc. This allows to maintain
sequence of words which is different as compared to just bag of words which does 
not maintain order of words.

* *Stopword List:* A list of empty words, with very little semantic values.
Deleting these terms avoids duplications and noise[@www-mari2011nlp].

* *Statistical evaluation:* NLP systems need to be evaluated for their efficiency,
accuracy and robustness. It can be done using below methods that do it in different 
ways [@www-nivre2002nlp].
*	*Descriptive Statistics:* This method calculates Word error rate, Accuracy rate,
Recall and Precision
*	*Estimation:* This method calculates confidence interval for true accuracy rate 
with certain probability.
*	*Hypothesis Testing:* When different NLP systems are applied to same set of data,
we want to compare their performance and suggest if one method is better than other.
This method allows us to do it by comparing certain performance parameter between two 
methods and performing hypothesis testing to tell if there is real statistical 
significance between the results or not.

## Linguistic processing of natural language

In the linguistic process, the words are determined to see 

:o: how can words see?

how they are related
and used together in making grammatical units, sentences etc. Parsers are 
created and applied to demonstrate the text's syntax structure. The method used to 
create the parser vary.
To determine the semantic structure of the words certain tools are used. The most
often used tool is the is the lexicographic database WordNet [@www-mari2011nlp].

> "This is an annotated semantic lexicon in different languages made up of synonym
groups called synsets which provide short definitions along with the different
semantic relationships between synonym groups[@www-mari2011nlp]."

## NLP for Big data

Big data is most text based content which constantly growing and is mostly 
unstructured (:o: grammar). Every industry generates a large volume of text information.
documents, notes, emails, patents, patient informations etc. As most of these
are text based data that is generated, Natural language process for big data
presents an opportunity to take advantage of the situation to reveal patterns,
and trends [@www-huddle2017nlp].

* *Interactions:* Interactive applications are becoming more and more common
these days like microsoft's cortana, smart phone assistants, language 
translation programs etc. These applications use natural language 
processing.

* *Business Intelligence:* Natural language process for big data enables the 
user to retrive the documents that they are looking not limited by searching 
for the documents with the exact keywords. NLP enables them to search using 
their own words and tries to retrieve the documents with that search.

* *Market Research:* With the growth of internet, social network is full 
of rich, noisy information. The brands and organizations can determine what
is said about their products and services by using the natural language 
processing for their market research analysis.

There are a lot of NLP libraries written, that helps (:o: grammar) in 
processing the big data [@www-fedak2018nlp].
Some of which are:

* *CoreNLP:*  It was originally written in java that can also support 
 multiple language like python. It is well known for its speed and its
 precise results [:o:].
 
* NLTK: Most commonly used NLP library. 
> Natural language tool kit's (NLTK) modular structure helps comprehend
the dependencies between components and get the firsthand experience with 
composing appropriate models for solving certain tasks [@www-fedak2018nlp]."

* *TextBlob:* Addition of components like sentiment analyzer becomes very 
easy with Textblob [:o:].

* *Gensim:* Used best for topic modeling and comparing the document 
similarity [:o:]

* *Spacy:* It is a new library which has a very high performance [:o:].

## NLP in Yelp data review

:o: What is yelp introductory paragraph incomplete

The first step in NLP depends on the application. Voice based systems like 
Google Assistant or Alexa translates words into text using Hidden Markov Models. 
The language and context is then understood through a series of coded grammar
rules that rely on algorithms that incorporate statistical machine learning. 
Another important step is Semantic analysis which helps interpret human 
sentences logically [@www-wikinlp]. 

We shall turn our focus on how this powerful 

:o: who claims it is powerful

technique could be used to interpret
restaurant reviews on Yelp through a sentiment analysis model. Here we will try to
predict whether a user liked a local business or not based on their
review on Yelp. A simple text classifier would (:o: grammar)
be built based on Python’s Pandas,
NLTK and Scikit-learn libraries. According to [@www-adam2018nlp], the plan would
be to start with a dataset containing 5000 reviews with the following info:

*	ID of the restaurant under review
*	ID of the posted review
*	Date the review was posted
*	The star rating provided.
*	The text for the review. 
  
NLTK library would be used to process the text and get basic information and
insight on the data. The next step would be to visualize the data by utilizing
histogram grids for every star rating. The goal would be to identify which feature
of the review is useful in finding correlations in the data frame. Once we derive
some useful correlations, they could be visualized. According to
[@www-terence2018nlp] Challenges faced in NLP text processing are:

*	Scalability and portability
*	Certain techniques are too expensive
*	Not very reliable as of now.
*	Speech/text processing.

## Installation

:o: why use an old version of python, why can we not use python 3.7

:o: why are you contardicting yourslef in the next sentence and than use python 3.5

1. Install Python 3.6. (avoid the 64-bit versions)
Install Numpy (optional):  (the version that specifies python3.5)

2. Install NLTK: pip install nltk

3. Test installation: ‘Start>Python35’, then type ‘import nltk’
install the NLTK packages:

:o: now you show us you use 3.5 yet you ask the user to use 3.6

```python
import nltk
nltk.download()
```

## Building a NLP pipeline

It would be really helpful if a computer could understand what the humans 
are trying to say. NLP helps the computer to read and understand all the 
data. By applying NLP techniques, we will be able to save a lot of time to 
the projects. But parsing the English langugae with a computer has its own
complications. Hence with NLP we will breakdown the process of understanding 
english, into small chunks and see how it performs in understanding and
giving a correct output [@www-adam2018nlp].

Let's take a paragraph: "Delhi is the capital of India and one of the
most populous city in Asia. This has been a great settlement for several
kings including the Mughals. The original name was Indraprastha." :o: if quotes are used they must be followed with a citation, otherwise you use italics

This paragraph contains several important and useful information. It would
be great if a computer could read and understand that Delhi is a city in 
India, it was ruled by Mughals etc. But to get there we have to train the 
computer on how to read the sentence [@www-adam2018nlp].

A lot of information in English is unstructured. 

:o: you repeat yourself?

For a computer to 
understand the text and extract data we need to do some of the following
steps [@www-adam2018nlp]:

* *Sentence Segmentation:*

First step is breaking the text in the paragraph into separate sentences like:

* "Delhi is the capital of India and one of the most populous city in Asia."

* "This has been a great settlement for several kings including the Mughals."

* "The original name was Indraprastha."

By breaking the text in the paragraph into small sentences it is easy for the 
computer to read understand them. We can use NLP pipeline methods to read 
the sentences and determine what it means.

* *Word Tokenization:*

Once we have broken the paragraph into sentences, we can process individual 
sentences. We can now break these sentences into separate words or tokens.
This is called "Tokenization"

```
Eg: "Delhi", "is", "the", "capital", "of", "India", "and", "one", "of", 
"the", "most", "populous", "city", "in", "Asia, "."
```
Every word including punctuation is split apart.

* *Predicting parts of speech:*

:o: indentation again wrong you again confuse markdown

Each token is taken individually and the part of speech for that token 
is determined. Finding out if the word is a noun, verb etc. helps to 
determine what the sentence is about.
Each word is fed into a part of speech classification model, which was 
trained already by feeding in millions of English sentences to determine
the words part of speech.

```
Eg: Delhi is a noun and capital is a noun. So we can determine that the 
sentence is probably about Delhi
```
* *Text Lemmatization:*

There may be cases where a same word may appear in different forms. Text 
Lemmatization helps to determine the base form of each word, so that it 
will be easy to figure out that the words are the same if they where in 
different base forms.

> "Lemmatization is typically done by having a look-up table of the lemma
forms of words based on their part of speech and possibly having some custom
rules to handle words that you’ve never seen before.[@www-adam2018nlp]"

* *Identifying Stop Words:*

There are lot of filler words like "a", "the" etc. These words are called stop
words. The stop words are considered a noise and are usually removed before 
performing any statistical analysis.

```
Eg: "Delhi", "capital", "India", "one", "most", "populous", "city", "Asia, "."
```
* *Dependency Parsing:*

Here we determine how the words are related to each other.

> "The goal is to build a tree that assigns a single parent word to each word
in the sentence. The root of the tree will be the main verb in the sentence .
In addition to determining the parent word, the relation that exists between
the word is also found out[@www-adam2018nlp]."

* *Finding noun phrases:*

The words that represent single idea is grouped together instead of considering
every word as a single entity. The information from the dependency parse
tree is taken to group the related words together.

Eg: By combining the non-phrases from the sentence we get:
```
"Delhi the capital most populous city ..."
```
* *Named Entity Recognition:*

The aim of Named Entity Recognition is to detect and label the nouns with 
real world concepts.

Eg: "Delhi", "India" and "Indraprastha" represent places on a map. With 
Named Entity Recognition we will be able to detect that on a map. 

A Named Entity can Recognize peoples name, location, products, date and time,
money etc.

## Example

Tokenize:

```python
from nltk.tokenize import sent_tokenize, word_tokenize
line = "A quick brown fox jumps over the lazy dog"
print(word_tokenize(line))
```

```
output: "A", "quick", "brown", "fox", "jumps", "over", "the", "lazy", "dog".
```
## Conclusion

Based on the user's query and information need, NLP system represents the true
meaning of what is expected. The content of the document will be searched in 
order to retrieve the relevant document based on the search query 
[@www-liddy1998nlp]. Alan Turing famously proposed a test to check intelligence
of machines. The test measures if a machine is able to exhibit intelligent 
behavior/thinking like humans when it is asked same question by a human and 
its response is compared to response of other human. This led to field of 
Artificial Intelligence (AI). NLP is important part of AI as it helps with
communication between machine and human.

## Team Members and work breakdown

  - Sahithya Sridhar (fa18-523-67): Introduction, Natural language text processing,
    Natural Language generation
  - Prajakta Patil (fa18-523-65): Related Work, Applications of NLP, NLP in 
    Yelp data review
