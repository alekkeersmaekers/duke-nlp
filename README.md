# duke-nlp
Automatically annotated papyrus texts, as used in the [Trismegistos Words](https://www.trismegistos.org/words) project. The original text data is from the [Duke Databank of Digital Papyri](https://github.com/papyri/idp.data) (downloaded from GitHub in September 2016), made available under a [Creative Commons Attribution 3.0 License](https://creativecommons.org/licenses/by/3.0/).

## Data format
The texts are divided into sentences and 'words' (i.e. tokens). For each token the following information is provided:
* wordref_id: a unique identifier for each tokenized word. Use this if you want to refer to individual words.
* id: the id of the word within the tokenized sentence.
* texid: the Trismegistos identifier of the text. See https://www.trismegistos.org/about_identifiers.php.
* row: row of the text on which the word appears, as specified in the DDbDP text.
* wordNum: place of the word on that row.
* hand: number of the 'hand' of the scribe(s).
* regularized: word form, as regularized by the editor.
* original: the word form that appears in the original text.
* completeness: measure of preservation of the text.
* tag: part-of-speech/morphology tag, consisting of a number of features.
* lemma: word lemma.
* lemmaFlag: automatically calculated field, referring to possible problems with the lemma.
* perseusTag: the part-of-speech tag in the format of the Perseus Treebanks.

## How to cite
This data is available under a [CC BY-SA 4.0 License](https://creativecommons.org/licenses/by-sa/4.0/). Please refer to the following paper when using this data:
> Keersmaekers, Alek, and Mark Depauw. Forthcoming. “Bringing Together Linguistics and Social History in Automated Text Analysis of Greek Papyri.” *Classics@*.
