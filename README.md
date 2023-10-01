# text-normalization-based-on-dictionary-cross-check

This notebook corrects every typos and/or slang words contained within the user's input by cross-checking each word against a dictionary.

Users can input via text through one endpoint & via .csv file through another, all within one API.

The dictionary used by this notebook is a .csv file named **new_kamusalay.csv**, source: https://github.com/okkyibrohim/id-multi-label-hate-speech-and-abusive-language-detection.
It contains two columns; the first one is the typo and slang words, and the second one is the formal words. Below is the mapping
* *beud --> banget*
* *jgn --> jangan*
* *loe --> kamu*

This notebook then counts the number of word & character of both the user's input & cleansed input and exports a .png file of the user's input's character count & cleansed input's character count comparison.

1) User's input, 2) its word count & 3) character count, 4) cleansed input, 5) its word count & 6) character count are then inserted into a .db database file, currently set as **database_Nasrudin.db**.

As the notebook file format implies, it uses python programming language & Jupyter Lab.

Citation:
**Muhammad Okky Ibrohim and Indra Budi. 2019. Multi-label Hate Speech and Abusive Language Detection in Indonesian Twitter. In *ALW3: 3rd Workshop on Abusive Language Online, 46-57*.** (Every paper template may have different citation writting. For LaTex user, you can see **citation.bib**).
