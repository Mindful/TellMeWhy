# TellMeWhy

Forked from https://github.com/Yeema/TellMeWhy so I can run it easier. 

<h2> Installation </h2>

1. pip install nltk flask spacy
2. pip install https://github.com/d2207197/geniatagger-python/archive/master.zip
3. Download Genia Tagger from http://www.nactem.ac.uk/GENIA/tagger/, place it into the same directory as TellMeWhy
4. cd into the Genia Tagger directory and run make
5. python -m spacy download en_core_web_md

<h2> Goal:</h2>
We introduce a method for learning to provide feedback on a given English sentence with a correction.
In our approach, the sentences and corrections are analyzed to identify the error type and a problem word, aimed at customizing explanations according to the context of the error type and the problem word.
The method involves identifying an error type and a problem word of the given sentence, generating common feedback patterns of each error type, and extracting grammar patterns along with collocations and example sentences for explanation. 
At run-time, a sentence with a correction is classified, and the problem word and template are identified to provide detailed explanations.
We present a prototype feedback system, \textit{TellMeWhy}, that applies the method to an annotated corpus and an underlying grammatical error correction system.
Preliminary evaluation on a set of representative sentences with common errors shows that the method has potential to outperform existing commercial writing services.

<h2> Usage:</h2>

cmd: python -m flask run -h 0.0.0.0 -p 9732
  