# Natural language text processing and Language generation :hand: fa18-523-67, fa18-523-65

| Sahithya Sridhar, Prajakta Patil
| sahsrid@iu.edu, patilpr@iu.edu
| Indiana University, Bloomington
| hid: fa18-523-67, fa18-523-65
| github: [:cloud:](https://github.com/cloudmesh-community/fa18-523-65/blob/master/paper/paper.md)
 
:o: not yet reviewd

## Introduction

> "The goal of NLP is to accomplish human-like language 
processing [@www-liddy1998nlp]".

Natural language processing (NLP) forms the link between machine language 
(binary code) to natural languages (which we humans speak). It borrows elements
from artificial intelligence, computer science and information engineering.
Success of NLP is highly dependent on how one can successfully program 
computers, to process, analyze and interpret huge amounts of natural language 
data. Key challenges/opportunities in this inter-disciplinary field involves 
speech recognition, language interpretation and generation of natural language
from a machine representation. With NLP, it is possible for computers to read
text, hear speech, interpret it, measure sentiment and determine which parts
are important [@www-sasnlp].

NLP was initially called NLU (Natural language understanding). A natural
language understanding system will be used to paraphrase the input text,
will be able to translate text into another language, analyse the content of
the text and draw conclusions.As NLP still cannot draw inference from the text,
it is still dependant on NLU. Based on the user's query and information need, 
NLP system represents the true meaning of what is expected. The content of 
the document will be searched inorder to retrieve the relevant document based 
on the search query [@www-liddy1998nlp].

## Natural language text processing

It is well known that quite a bit information which exists out in our world is
very unstructured. The challenge would be to make a computer to understand this
and extract data from it. Take English language as an example. Humans have been
writing down things for thousands of years but computers can’t yet truly
understand the language as we do. The trick is to break down the process of
understanding English into smaller chunks and understanding each smaller piece
separately [@www-sasnlp].

According to [@www-liddy1998nlp] Natural language processing has two distinct
focuses:
* *Language processing:* Produces a meaningful representation by analysing the 
 language 
* *Language generation:* language is produced from representation.This requires
 a planning capability. 
 

The text is manipulated for abstractions and indexed for automatic knowledge
extraction. Producing text in a desirable format is one of the major research
areas in NLP. structuring of large bodies of textual information to retrieve a
information is classified under the Natural language text processing
[@www-liddy1998nlp].
> "The central
task for natural language text processing systems is the translation of
potentially ambiguous natural language queries and texts into unambiguous
internal representations on which matching, and retrieval can take place"
[@www-liddy1998nlp].

## Levels of NLP

Past research concentrating on natural language text processing systems has been
reviewed by many [@www-haas1996nlp].
The various important terminologies of Natural Language Processing are: 

 * *Phonology:* refers to the systematic arrangement of sound. There are three 
         types of rules used here: 
         
    > "* *phonetic rules:* for sounds within words; 
       * *phonemic rules:* for variations of pronunciation when words are spoken 
          together, and
       * *prosodic rules:* for fluctuation in stress and intonation
          across a sentence [@www-liddy1998nlp]."
     
* *Morphology:* comprises of nature of words where the different parts of the
  words represent smallest units. A word can be broken down into its 
  constituent morphemes to understand the meaning [@www-liddy1998nlp].
*	*Lexical:* Interprets the meaning of the sample word. Words that have only 
   one meanings is replaced by the semantic representation of a word. This 
   requires the word to have a simple or a complex lexicon [@www-liddy1998nlp].
*	*Syntactic:* Rectifies the grammatical mistakes in a sentence. The output 
   reveals a that has a structural dependancy between the words.Variours 
   grammars are used which inturn affects the choice of the parser.As the order 
   of the words convey different meanings syntax conveys meanings in most 
   languages [@www-liddy1998nlp].
*	*Semantic:* determines the meaning of the word by pivoting on the interactions
  among word-level meanings in the sentence.
*	*Discourse:* Focusses on properties of the text that convey meaning by making
  connections between component sentences.
  
  >"Discourse/text structure recognition determines the functions of sentences in
    the text, which, in turn, adds to the meaningful representation of the text"
    [@www-liddy1998nlp].
    
* *Pragmatic:* It is concerned with the firm use of the language.The main
   goal is the use of the context over the content of the text
   for understanding. This determines how extra word is read into
   the text with the words encoded in the sentance[@www-chaudhary2003nlp]. 
   
Current NLP system tends to implement those models that are used for 
processing the lower levels as they have been well researched and implemented
and also the apllications do not require them to process at the higher levels
[@www-liddy1998nlp].

## Natural Language generation

According to [@www-khurana2017nlp] the NLP happens in four phases:
*	Identifying the goal
*	Evaluating the situation and planning to achieve the goal
*	Evaluate the available resources.
*	Execute the plans as text.

## Approaches to NLP:

According to [@www-liddy1998nlp] some approaches of NLP are as follows:

* *Symbolic Approach-* Performs deep analysis of linguistic phenomena based on 
   the human developed rules and lexicons. Logic or rule based systems and 
   semantic networks are good examples of symbolic approach.
   
   >"Symbolic approaches have been used for a few decades in a variety of research
   areas and applications such as information extraction, text categorization, 
   ambiguity resolution, and lexical acquisition [@www-liddy1998nlp]"
   
* *Statistical Approach-* Various mathematical techiques are used here. Observable 
   data is used mainly as evidence. Hidden markov model is a widely used
   statistical approach. This is used in speech recognition, parsing, statistical
   grammar learning etc
   
* *Connectionist-* Models are developed based on the linguistic phenomena. This 
   combines statistical model with other theories.
   

## Related Work

Researchers working on NLP, building tools and systems which makes NLP what it
is today. Tools like Sentiment Analyzer, parts of speech, Emotion detection,
Semantic Role Labelling etc made NLP a good topic for research.

* *Sentiment Analyzer:* analyses the document for positive and negative words.
  It uses the sentiment lexicon and the sentiment pattern database to analyze the
  sentiments.

* *Parts of speech:* It can efficiently tag and classify words as nouns, adjectives,
  verbs etc. Taggers are already present for the  European languages, research is
  being done on making parts of speech taggers for other languages like Arabic,
  Sanskrit [@www-tapaswi2012nlp], Hindi [@www-ranjan2003nlp] etc.
  
* *Emotion Detection:* This is like sentiment analysis, but it works on social media
  platforms on mixing of two languages. It categorizes statements into six groups
  based on emotions [@www-khurana2017nlp].

* *Sematic Role Labelling:* SRL works by giving a semantic role to a sentence.
  like assigning roles to words that are arguments of a verb in the sentence
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

* *Text categorization:* splitting the large volume of data into several categories.
  Example spam filters. 

* *Spam Detection:* Various machine learning techniques like Rule Learning,
  Naïve Bayes, Memory based Learning, Support vector, Decision Trees,
  Maximum Entropy Model etc are used to detect the spams.This is very similar to 
  text categorization.
  
## Problems with natural language processing: linguistic variation and ambiguity 

There are certain problems is natural language processing that reduce the efficacy 
of textual information retireval. linguistic variation and ambiguity are some of 
the problems in NLP. Linguistic variation is an issue when the same words or 
expressions are used to communicate the idea. Multiple interpretations is the 
main problem with Linguistic variation.Linguistic Variation provokes the 
omission of certain documents that are relevant and Ambiguity implies when a 
document has duplicate words or words that are not related [@www-mari2011nlp].

* *Example 1: A notebook was the present that the teacher gave him, when we where
present in the class.*

Here the word "present" has different meanings both as an adjective and as a noun.
The word present plays different morph-syntactic depending on the situation,
causing ambiguity problems.

* *Example 2: He ate food on the car.*

Ambiguity is produced here again, as this sentence can have several meanings 
like, he ate the food which was present in the car,or he ate food when he was 
driving the car.

* *Example 3: I went to the bank.*

Here the bank could mean a place where save mony and transcations are made or
a mound.

These examples show that automated process is not easy and that how complex the
language is.

## Natural Language processing in textual information retrieval

When the user gives a query the following task are performed as a part of 
Natural Language processing's textual information retrieval:

* Index is created for the descriptions of a document based on the NLP
techniques.

* When a query is given by a user the system analyses it and transforms it
such that it is similar to what is represented in the document.

* The description of each document is comapred by the system with the query
given by the user, and those documents that have the description close to the 
users query to retrieved.

* The results are shown in the order of the similarity.
[@www-mari2011nlp]

## Statistical processing of natural language

> "This is a very simple focus based on the "bag of words." In this approach,
all words in a document are treated as its index terms. Moreover, each term is
assigned a weight in function of its importance, usually determined by its 
appearance frequency within the document. This way the word's order, structure,
meaning, etc, are not taken into consideration [@www-mari2011nlp]."

The document processing model involves document pre-processing and Parameterisation.

* *Document pre-processing:* Prepares the documents by removing those elements that
are superfluous.There are three basic phases here:

   * Removing headers, tags etc from the document which are not for indexing.
   * Standardising the text by checking for capitalized or non-capitalized
   letters, numerals, dates etc.
   * Stemming the terms by reducing the words to the roots.

* *Parameterisation:* >"quantifying the document's characteristics
 [@www-mari2011nlp]."

   * Assigns weights to the  relevant terms present in the document.

One of the most used methods to estimate the importance of a term is the TFIDF
system (Term Frequency, Inverse Document Frequency).

>"It is designed to calculate the importance of a term relative to its appearance
frequency in a document, but as a function of the total appearance frequency for
all of the corpus' documents. That is, the fact that a term appears often in one
document is indicative that that term is representative of the content, but only
when that term does not appear frequently in all documents. If it appeared frequently
in all documents, it would not have any discriminatory value [@www-mari2011nlp]."

Two commonly used techniques in statistical processing is:

* *Detecting N-Grams:* This involves identifying compound words, proper nouns etc,
to be able to process them as single words. This is done by determining the 
probability of the compound words like European union etc.

* *Stopword List:* A list of empty words, with very little semantic values.
Deleting these terms avaids duplications and noise[@www-mari2011nlp].

## Linguistic processing of natural language

In the linguistic process, the words are determined to see how they are related
and used together in making gramatical units , sentences etc. Parsers are 
created and applied to demonstrate the text's syntax structure. The method used to 
create the parser vary.
To determine the semantic structure of the words certain tools are used. The most
often used tool is the is the lexicographic database WordNet [@www-mari2011nlp].

>"This is an annotated semantic lexicon in different languages made up of synonym
groups called synsets which provide short definitions along with the different
semantic relationships between synonym groups[@www-mari2011nlp]."

## NLP in Yelp data review

The first step in NLP depends on the application. Voice based systems like 
Google Assistant or Alexa translates words into text using Hidden Markov Models. 
The language and context is then understood through a series of coded grammar
rules that rely on algorithms that incorporate statistical machine learning. 
Another important step is Semantic analysis which helps interpret human 
sentences logically [@www-wikinlp]. 

We shall turn our focus on how this powerful technique could be used to interpret
restaurant reviews on Yelp through a sentiment analysis model. Here we will try to
predict whether a user liked a local business or not based on their
review on Yelp. A simple text classifier would be built based on Python’s Pandas,
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
of the review is useful in finding correlations in the dataframe. Once we derive
some useful correlations, they could be visualized.According to
[@www-terence2018nlp] Challenges faced in NLP text processing are:

*	Scalability and potability
*	Certain techniques are too expensive
*	Not very reliable as of now.
*	Speech/text processing.

## Installation

1. Install Python 3.6. (avoid the 64-bit versions)
Install Numpy (optional):  (the version that specifies python3.5)

2. Install NLTK: pip install nltk

3. Test installation: ‘Start>Python35’, then type ‘import nltk’
install the NLTK packages:

```python
import nltk
nltk.download()
```

## Building a NLP pipeline

It would be really helpful if a computer could understand what the humans 
are trying to say. NLP helps the computer to read and understand all the 
data. By applying NLP techniques, we will be able to save a lot of time to 
the projects. But parsing the english langugae with a computer has its own
complications.Hence with NLP we will breakdown the process of understanding 
english, into small chunks and see how it performs in understanading and
giving a correct output [@www-adam2018nlp].

Lets take a para: "Delhi is the capital of India and one of the
most populous city in Asia. This has been a great settlement for several
kings including the Mughals. The original name was Indraprastha."

This para contains several important and useful information. It would
be great if a computer could read and understand that Delhi is a city in 
India, It was ruled by Mughals etc. But to get there we have to train the 
computer on how to read the sentence [@www-adam2018nlp].

A lot of information in english is unstructured. For a computer to 
understand the text and extract data we need to do some of the following
steps [@www-adam2018nlp]:

* *Sentence Segmentation:*

First step is breaking the text in the para into seperate sentences like:

* "Delhi is the capital of India and one of the most populous city in Asia."

* "This has been a great settlement for several kings including the Mughals."

* "The original name was Indraprastha."

By breaking the text in the para into small sentences it is easy for the 
computer to read understand them. We can use NLP pipeline methods to read 
the sentences and determine what it means.

* *Word Tokenization:*

Once we have broken the para into sentences, we can process individual 
sentences. We can now break these sentences into eperate words or tokens.
This is called "Tokenization"

Eg: "Delhi", "is", "the", "capital", "of", "India", "and", "one", "of", 
"the", "most", "populous", "city", "in", "Asia, "."
Every word including punctuation is split apart.

* *Predicting parts of speech:*

Each token is taken individually and the part of speech for that token 
is determined. Finding out if the word is a noun, verb etc helps to 
determine what the sentence is about.
Each word is fed into a part of speech classification model, which was 
trained already by feeding in millions of english sentences to determine
the words part of speech.

Eg: Delhi is a noun and capital is a noun. So we can determine that the 
sentence is probably about delhi

* *Text Lemmatization:*

There may be cases where a same word may appear in different forms. Text 
Lemmatization helps to determine the base form of each word, so that it 
will be easy to figure out that the words are the same if they where in 
different base forms.

> "Lemmatization is typically done by having a look-up table of the lemma
forms of words based on their part of speech and possibly having some custom
rules to handle words that you’ve never seen before.[@www-adam2018nlp]"

* *Identifying Stop Words:*

There are lot of filler words like "a","the" etc. These words are called stop
words. The stop words are considered a noise and are usually removed before 
performing any statistical analysis.

Eg: "Delhi", "capital", "India", "one", "most", "populous", "city", "Asia, "."

* *Dependency Parsing:*

Here we determine how the words are related to each other.

> "The goal is to build a tree that assigns a single parent word to each word
in the sentence. The root of the tree will be the main verb in the sentence 
[@www-adam2018nlp]."

In addition to determining the parent word, the relation that exists between
the word is also found out.

* *Finding noun phrases:*

The words that represent single idea is grouped together instead of considering
every word as a single entity. The information from the dependancy parse
tree is taken to group the related words together.

Eg: By combining the non phrases from the sentance we get:

"Delhi the capital most populous city ..."

* *Named Entity Recognition:*

The aim of Named Entity Recognition is to detect and label the nouns with 
real world concepts.

Eg: "Delhi", "India" and "Indraprastha" represent places on a map. With 
Named Entity Recognitio we will be able to detect that on a map. 

A Named Entity can Recognise peoples name, location, products, date and time,
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

## Team Members and work breakdown

  - Sahithya Sridhar (fa18-523-67): Introduction, Natural language text processing,
    Natural Language generation
  - Prajakta Patil (fa18-523-65): Related Work, Applications of NLP, NLP in 
    Yelp data review
