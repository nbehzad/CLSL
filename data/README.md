# Resource description

There are three main folders in the data directory namely external-resources', <system-generated-resources> and 'output'.

## external-resources

<external-resources> folder includes all external resources needed for the construction of the model. It consists of 3 kinds of resources containing in 3 folders as below:

### parallel-corpora 

<parallel-corpora> folder includes all parallel subtitle texts. In this folder, for each target language, a folder named “en-targetID`` (e.g. en-de) exists to store the two separate files of parallel subtitle texts. It means that the lines of two files are equivalent to (translation of) each other. The below convention is used in the name of files:
 “targetID-opensubtitle.txt” e.g. for two pair language English-German, two files are available: <de-opensubtitle.txt> and <de-opensubtitle.txt>
 
### source-sentiment-lexicon

The SentiWordNet lexicon are available in the <source-sentiment-lexicon> folder. This file has been downloaded from (http://sentiwordnet.isti.cnr.it/).

### filtered-vocab

The folder <filtered-vocab> includes all term-list of different languages that should be excluded in the indexing phase, e.g. stop-words. However, all these terms should be collected in a single text file such that each line is a single term. File naming convention is as follows: <targetID-fv.txt> e.g. de-fv.txt for German.

## system-generated-resources

<system-generated-resources> folder is used to store the resources produced by the system. As the indexing phase might be time-consuming, system saves the indexed file and reuses it in the next runs 

## output

The target sentiment lexicons are generated in the <output> folder. For each target language 4 types of lexicons are generated based on methods used to conflate the polarities of the mapped synsets.

