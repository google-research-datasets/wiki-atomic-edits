# WikiAtomicEdits

A dataset of atomic wikipedia edits containing insertions and deletions of a contiguous chunk of text in a sentence. This dataset contains ~43 million edits across 8 languages.

## Description

An atomic edit is defined as an edit *e* applied to a natural language expression *S* as the insertion, deletion, or substitution of a sub-expression *P* such that both the original expression S and the resulting expression *e(S)* are well-formed semantic constituents (MacCartney, 2009). In this corpus, we release such atomic insertions and deletions made to sentences in wikipedia.

Following are the number of examples by language:

Language | Insertions | Deletions |
---------|------------|-----------|
German  | 3.3  | 1.9 |
English | 13.7 | 9.3 |
Spanish | 1.4  | 0.9 |
French  | 2.0  | 2.0 |
Italian | 1.0  | 0.6 |
Japanese| 2.2  | 1.3 |
Russian | 1.4  | 0.9 |
Chinese | 0.7  | 0.4 |
Total   | 25.7 | 17.2|

## Examples

Example of an insertion:

*She died there after a long illness.* + *in 1949* = *She died there in 1949 after a long illness.*

Example of a deletion:

*She dreams about entering the Black Lodge and about a ring.* - *and about a ring.* = *She dreams about entering the Black Lodge.*

For each language we provide two files, one each for insertions and deletions. The files contains the following tab-separated columns:

Column | Data |
:-----:| -----|
1      | Original sentence |
2      | Insertion/deletion|
3      | Edited sentence   |

## Reference 

If you use or discuss this dataset in your work, please cite our paper:

```
@InProceedings{WikiAtomicEdits,
  title = {{WikiAtomicEdits: A Multilingual Corpus of Wikipedia Edits for Modeling Language and Discourse}},
  author = {Faruqui, Manaal and Pavlick, Ellie and Tenney, Ian and Das, Dipanjan},
  booktitle = {Proc. of EMNLP},
  year = {2018}
}
```

## License

Query-wellformedness dataset is licensed under [CC BY-SA 4.0](http://creativecommons.org/licenses/by-sa/4.0/). Any third party content or data is provided “As Is” without any warranty, express or implied.

## Contact

If you have a technical question regarding the dataset or publication, please
create an issue in this repository.
