# duke-nlp
Automatically annotated papyrus texts, as used in the [Trismegistos Words](https://www.trismegistos.org/words) project. The original text data is from the [Duke Databank of Digital Papyri](https://github.com/papyri/idp.data) (downloaded from GitHub in September 2016), made available under a [Creative Commons Attribution 3.0 License](https://creativecommons.org/licenses/by/3.0/).

**New: syntactic parsing and semantic role labeling.** SRL is still in the experimental stage. Morphological tagging accuracy is estimated to be about 95%, lemmatization 99%, syntactic parsing 85%-90%, and semantic role labeling 81% for everyday texts (letters, petitions) - the results for the other texts should be used with more caution. The files are now combined into larger files for practical purposes, but the original XMLs can be retrieved with the "filename" attribute. The language-external information is included from the Trismegistos databases (https://www.trismegistos.org).

## Data format
The texts are divided into sentences and 'words' (i.e. tokens). For each token the following information is provided:
* id: the id of the word within the tokenized sentence.
* wordid: a unique identifier for each tokenized word. Use this if you want to refer to individual words.
* row: row of the text on which the word appears, as specified in the DDbDP text.
* wordNum: place of the word on that row.
* hand: number of the 'hand' of the scribe(s).
* regularized: word form, as regularized by the editor.
* form: the word form that appears in the original text.
* completeness: measure of preservation of the text.
* texid: the Trismegistos identifier of the text. See https://www.trismegistos.org/about_identifiers.php.
* lemma: word lemma.
* postag: part-of-speech/morphology tag, in the format of the Ancient Greek Dependency Treebanks.
* head: head word in the syntactic tree.
* relation: syntactic label, as used in the Ancient Greek Dependency Treebanks.
* lemmaFlag: automatically calculated field, referring to possible problems with the lemma.
* perseusTag: the part-of-speech tag in the format of the Perseus Treebanks.
* semanticRole: semantic role label.

## How to cite
This data is available under a [CC BY-SA 4.0 License](https://creativecommons.org/licenses/by-sa/4.0/). Please refer to the following paper when using this data:
> Keersmaekers, Alek, and Mark Depauw. Forthcoming. “Bringing Together Linguistics and Social History in Automated Text Analysis of Greek Papyri.” *Classics@*.
