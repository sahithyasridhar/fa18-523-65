# Natural language text processing and Language generation :hand: fa18-523-67, fa18-523-65

| Sahithya Sridhar, Prajakta Patil
| sahsrid@iu.edu, patilpr@iu.edu
| Indiana University, Bloomington
| hid: fa18-523-65, fa18-523-67
| github: [:cloud:](https://github.com/cloudmesh-community/fa18-523-65/blob/master/paper/paper.md)
 
:o: not yet reviewd

## Introduction

>"The goal of NLP as stated above is “to accomplish human-like language 
processing"
Natural language processing (NLP) forms the link between machine language 
(binary code) to natural languages (which we humans speak). It borrows elements
from artificial intelligence, computer science and information engineering.
Success of NLP is highly dependent on how one can successfully program computers,
to process, analyze and interpret huge amounts of natural language data. Key
challenges/opportunities in this inter-disciplinary field involves speech 
recognition, language interpretation and generation of natural language from a
machine representation. With NLP, it is possible for computers to read text, hear
speech, interpret it, measure sentiment and determine which parts are important
[@fa18-523-67-www-google-2].

NLP was initially called NLU (Natural language understanding). A natural
language understanding system will be used to paraphrase the input text,
will be able to translate text into another language, analyse the content of
the text and draw conclusions.As NLP still cannot draw inference from the text,
it is still dependant on NLU.
Based on the user's query and information need, NLP system represents the true
meaning of what is expected. The content of the document will be searched 
inorder to retrieve the relevant document based on the search query.

## Natural language text processing

It is well known that quite a bit information which exists out in our world is
very unstructured. The challenge would be to make a computer to understand this
and extract data from it. Take English language as an example. Humans have been
writing down things for thousands of years but computers can’t yet truly
understand the language as we do. The trick is to break down the process of
understanding English into smaller chunks and understanding each smaller piece
separately [[@fa18-523-67-www-google-2].

Natural language processing has two distinct focuses:
* *Language processing:* Produces a meaningful representation by analysing the 
 language 
* *Language generation:* language is produced from representation.This requires
 a planning capability. 

The text is manipulated for abstractions and indexed for automatic knowledge
extraction. Producing text in a desirable format is one of the major research
areas in NLP. structuring of large bodies of textual information to retrieve a
information is classified under the Natural language text processing.
> "The central
task for natural language text processing systems is the translation of
potentially ambiguous natural language queries and texts into unambiguous
internal representations on which matching, and retrieval can take place"
[@fa18-523-67-NLP-1].

## Levels of NLP

Past research concentrating on natural language text processing systems has been
reviewed by many [@fa18-523-67-NLP-2].Some of the Terminologies used are:

The various important terminologies of Natural Language Processing are: -
* *Phonology-* refers to the systematic arrangement of sound. There are three 
  types of rules used here: 
  >"-phonetic rules – for sounds within words; 
    -phonemic rules – for variations of pronunciation when words are spoken 
     together, and
    -prosodic rules – for fluctuation in stress and intonation
     across a sentence"
* *Morphology-* comprises of nature of words where the different parts of the
  words represent smallest units. A word can be broken down into its 
  constituent morphemes to understand the meaning.
*	*Lexical-* Interprets the meaning of the sample word. Words that have only 
   one meanings is replaced by the semantic representation of a word. This 
   requires the word to have a simple or a complex lexicon.
*	*Syntactic-* Rectifies the grammatical mistakes in a sentence. The output 
   reveals a that has a structural dependancy between the words.Variours 
   grammars are used which inturn affects the choice of the parser.As the order 
   of the words convey different meanings syntax conveys meanings in most 
   languages.
*	*Semantic-* determines the meaning of the word by pivoting on the interactions
  among word-level meanings in the sentence.
*	*Discourse-* Focusses on properties of the text that convey meaning by making
  connections between component sentences.
  >"Discourse/text structure recognition determines the functions of sentences in
    the text, which, in turn, adds to the meaningful representation of the text"
    [@fa18-523-67-NLP-3].
* *Pragmatic-* It is concerned with the firm use of the language.The main
   goal is the use of the context over the content of the text
   for understanding. This determines how extra word is read into
   the text with the words encoded in the sentance[@fa18-523-67-NLP]. 
   
   Current NLP system tends to implement those models that are used for 
   processing the lower levels as they have been well researched and implemented
   and also the apllications do not require them to process at the higher levels.

## Natural Language generation

This happens in four phases:
*	Identifying the goal
*	Evaluating the situation and planning to achieve the goal
*	Evaluate the available resources.
*	Execute the plans as text [@fa18-523-67-NLP-Art].

## Approaches to NLP:

* *Symbolic Approach-* Performs deep analysis of linguistic phenomena based on 
   the human developed rules and lexicons.Logic or rule based systems and 
   semantic networks are good examples of symbolic approach.
   >"Symbolic approaches have been used for a few decades in a variety of research
   areas and applications such as information extraction, text categorization, 
   ambiguity resolution, and lexical acquisition"
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
  Sanskrit [@fa18-523-67-NLP-Art-1], Hindi [@fa18-523-67-NLP-Art-2] etc.
  
* *Emotion Detection:* This is like sentiment analysis, but it works on social media
  platforms on mixing of two languages. It categorizes statements into six groups
  based on emotions [@fa18-523-67-NLP-Art-3].

* *Sematic Role Labelling:* SRL works by giving a semantic role to a sentence.
  like assigning roles to words that are arguments of a verb in the sentence
  [@fa18-523-67-NLP-Art-4].

## Applications of NLP

Natural Language Processing can be applied into various areas like Machine
Translation, Email Spam detection, Information Extraction, Summarization,
Question Answering etc.

* *Machine Translation:* As the name suggests Machine translation is translating a
  phrase from one language to another with the help of engines like google
  translate. The major challenge in machine translation is keeping the meaning and
  the grammatical structure of the translated language intact.

* *Text categorization:* splitting the large volume of data into several categories.
  Example spam filters. 

* *Spam Detection:* Various machine learning techniques like Rule Learning,
  Naïve Bayes, Memory based Learning, Support vector, Decision Trees,
  Maximum Entropy Model etc are used to detect the spams.This is very similar to 
  text categorization [@fa18-523-67-NLP-Art].

## NLP in Yelp data review

The first step in NLP depends on the application. Voice based systems like Google
Assistant or Alexa translates words into text using Hidden Markov Models. 
The language and context is then understood through a series of coded grammar
rules that rely on algorithms that incorporate statistical machine learning. 
Another important step is Semantic analysis which helps interpret human 
sentences logically [@fa18-523-67-www-google-1]. 

We shall turn our focus on how this powerful technique could be used to interpret
restaurant reviews on Yelp through a sentiment analysis model. The goal of this
paper is to predict whether a user liked a local business or not based on their
review on Yelp. A simple text classifier would be built based on Python’s Pandas,
NLTK and Scikit-learn libraries. The plan would be to start with a dataset
containing 5000 reviews with the following info:

*	ID of the restaurant under review
*	ID of the posted review
*	Date the review was posted
*	The star rating provided.
*	The text for the review [@fa18-523-67-www-google-3].

NLTK library would be used to process the text and get basic information and
insight on the data. The next step would be to visualize the data by utilizing
histogram grids for every star rating. The goal would be to identify which feature
of the review is useful in finding correlations in the dataframe. Once we derive
some useful correlations, they could be visualized.Challenges faced 
in NLP text processing:

*	Scalability and potability
*	Certain techniques are too expensive
*	Not very reliable as of now.
*	Speech/text processing [@fa18-523-67-www-google-4].

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
