# Resource description

There are three main folders in the data directory namely 'external-resources', 'system-generated-resources' and 'output'.

## 1. external-resources

The 'external-resources' folder includes all external resources needed for the construction of the model. It consists of 3 kinds of resources containing in 3 folders as below:

### 1.1 parallel-corpora 

This folder includes all parallel subtitle texts. For each target language, a folder named 'en-targetId' (e.g. en-de) exists to store the two separate files of parallel subtitle texts. It means that the lines of two files are equivalent to (translation of) each other. The below convention is used in the name of files:
 'targetId-opensubtitle.txt' e.g. for a pair language English-German, two files are available: <de-opensubtitle.txt> and <de-opensubtitle.txt>
 
### 1.2. source-sentiment-lexicon

The SentiWordNet lexicon is available in this folder. It has been downloaded from (http://sentiwordnet.isti.cnr.it/).

### 1.3 filtered-vocab

The folder 'filtered-vocab' includes all term-list of source-target languages that should be excluded in the indexing phase, e.g. stop-words. However, each of term lists should be collected in a single text file such that each line is considered as a single term. File name convention is as follows: 

<targetId-fv.txt> e.g. de-fv.txt for German.

## 2. system-generated-resources

This folder is used to store the resources produced by the system. As the indexing phase might be time-consuming, system saves the indexed file and reuses it in the next runs.

## 3. output

The target sentiment lexicons will be generated in this folder. For each target language 4 types of lexicons are generated based on the methods employed in conflating the polarities of the mapped synsets.

