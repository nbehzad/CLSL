# CLSL
CLSL (Cross Lingual Sentiment Lexicon) is a system to generate sentiment lexicons for multilingual sentiment analysis.
This system has been developed in .Net framework and its source codes will be published in the near future.

Here there is a compiled version of the system for creating a sentiment lexicon for German. The detail of the system will be published soon.

You can find the pre-constructed lexicons in the <./lexicons> directory.

# Usage
All system requirements are available in <./data> directory. Please see the README.md in this directory.  

Go to the <bin/Release> directory and Run the <MultiLexConstruction.exe> file as below:
It has 2 parameters: (1)target language id (e.g. <de> for German) (2) an integer indicating the vector reduction size. 

```
MultiLexConstruction de 10
```
The lexicons will be created in the <data/output> directory. 
 