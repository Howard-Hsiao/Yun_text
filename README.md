# Yun_text
Yun text is a text mining tool that support the user to do the basic text mining task. Currently, this package allows users to compute the variable numerical statistics of the given document or corpus.

## Prequisite
You should ensure that you have install the following dependencies. If you have not done so, you can follow the following instructions to install them.

```shell
# in the shell
pip install --user -U nltk
```

```python
# in python
import nltk
nltk.download("punkt")
nltk.download("stopwords")
```

## Python version support
Officially Python 3.6.1 and above, 3.7, and 3.8.

## How to use
1. Download the code  
```shell
git clone https://github.com/Howard-Hsiao/Yun_text.git
```
2. Move the whole directory "/src/Yun_text" to the same folder where the code using it exist

## supporting function and examples
* compute tf-idf
```python
from Yun_text.termMachine import termMachine
termMachineA = termMachine("path_of_1_document")
print(termMachineA.tf_dict)
```

* compute cosine similarity of 2 words using tf-idf
```python
from Yun_text.dictionary import Dictionary
dictionary = Dictionary(source=["path_of_1_document",
                                "folder of multiple documents",
                                []])
print(dictionary.cosine("word1", "word2"))
```

## The more detailed function of each module can be checked in the link below
* [termMachine](./doc/termMachine.md)
* [Dictionary](./doc/Dictionary.md)
