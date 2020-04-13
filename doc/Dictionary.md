#dictionary
## Introduction
When computing the tf-idf of a word, if the df of that word is equal to the documentNum, the its tf-idf is not 0. I add 0.1 to all of the word's tf-idf to avoid 0 propagation.

## Initialization
```
@param collection: the source of document, whose term would be extracted.
    the collection can be
    > a path of a directory that contain a series of raw text files
    > a path of a raw text file
    > a query string
    > a list containing stuff mentioned above
```

## Features
### Property
* source: the list that record the source
* documentNum: the number of the source
* centroid

### Function
```
cosine(self, word1, word2)
@target: calculate the cosine similarity of word1 and word2
---
@param: word1, word2:
    > the return value of Dictionary.get_tf_idf()
    > Dictionary.centroid
    > documentName
[Warning]: This function do not checkt the arguments are of legal type.
```

```
save_tf_idf(self, Doc, FileName="DocID.txt", sep = ", ", end = "\n"):
    save the result.
```

```
save_dict(self, FileName="dictionary.txt"):
    save the dictionary
```

```
addNewSource(self, newCollection):
    manually update the Dictionary with new collection
```

### extra Features
we can add multiple Dictionary to get a larger Dictionary with '+', '+='
