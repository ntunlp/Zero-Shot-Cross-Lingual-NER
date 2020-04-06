# Zero-Shot-Cross-Lingual-NER

Repository for [`Zero-Resource Cross-Lingual Named Entity Recognition`](https://arxiv.org/abs/1911.09812) AAAI'20 paper.

# News 

- Dataset released
    - dataset for finnish (fi) and arabic (ar) is updated. Please check [here](https://github.com/ntunlp/Zero-Shot-Cross-Lingual-NER/tree/master/ner_data).
    - the remaining datasets are from conll `en`, `es`, `de` and `nl`. They are available in the respective source. 


**Warning :** The full content of the repository is not yet updated. 
Codes and pretrined model will be release in a few weeks ... 

**Update :** Will be updating the codebase as soon as I got the licence. (delayed due to covid-19 scenario). In the mean time if you need any details please mail me from [here](https://sbmaruf.github.io/). I would love to help for any details. Sorry for the inconvenience. 

## Language short form

| Language | Three letter | Standard |
|---------|-----|----|
| English | eng | en |
| Spanish | esp | es |
| Dutch   | ned | nl |
| German  | deu | de |
| Arabic  | arb | ar |

This repository uses standard short form of the languages. Note: conll uses three letter short form. 


# Dataset

1. English (en) : [`CoNLL-2003 shared task`](https://www.aclweb.org/anthology/W03-0419.pdf).

2. Spanish (es) : [`CoNLL-2002 shared task`](https://www.aclweb.org/anthology/W02-2024.pdf).

3. Dutch (es) : [`CoNLL-2002 shared task`](https://www.aclweb.org/anthology/W02-2024.pdf).

4. German (de) : [`CoNLL-2003 shared task`](https://www.aclweb.org/anthology/W03-0419.pdf)

5. finnish (fi) : Adapted from [this](https://github.com/mpsilfve/finer-data) repository. However, they don't come in a form so that we can perform transfer learning experiments (from en conll NER dataset to fi dataset). We refactored the original source and corrected some tags manually for standardization.

6. Arabic (ar) : Adapted from [here](http://www.cs.cmu.edu/~ark/ArabicNER/). However, they don't come in a form so that we have a proper train, dev, test split. Dataset comes with 28 manually annotated wikipedia articles. For train, dev and test split creation, we randomly select sentences from each of the article and add it to a train, dev and test split. Split size, train(~90%), dev(~10%), test(~10%). Few tags and/or tokens are manually altered for standardization so that we can perform transfer learning experiments.




 

If you are using `refined` Finnish NER dataset please cite the following papers,

```
@inproceedings{bari19,
	Address     = {New York, USA},
	Author      = {M Saiful Bari and Shafiq Joty and Prathyusha Jwalapuram},
	Booktitle   = {Proceedings of the 34th AAAI Conference on Artificial Intelligence},
	Numpages    = {},
	Publisher   = {AAAI},
	Series      = {AAAI '20},
        pages       = {xx--xx},
	Title       = {{Zero-Resource Cross-Lingual Named Entity Recognition}},
	Year        = {2020},
	url         = {}
}
```
```
@article{Ruokolainen_2019,
   title={A Finnish news corpus for named entity recognition},
   ISSN={1574-0218},
   url={http://dx.doi.org/10.1007/s10579-019-09471-7},
   DOI={10.1007/s10579-019-09471-7},
   journal={Language Resources and Evaluation},
   publisher={Springer Science and Business Media LLC},
   author={Ruokolainen, Teemu and Kauppinen, Pekka and Silfverberg, Miikka and Lindén, Krister},
   year={2019},
   month={Aug}
}
```

If you are using `refined` Arabic NER dataset please cite the following papers,

```
@inproceedings{bari19,
	Address     = {New York, USA},
	Author      = {M Saiful Bari and Shafiq Joty and Prathyusha Jwalapuram},
	Booktitle   = {Proceedings of the 34th AAAI Conference on Artificial Intelligence},
	Numpages    = {},
	Publisher   = {AAAI},
	Series      = {AAAI '20},
        pages       = {xx--xx},
	Title       = {{Zero-Resource Cross-Lingual Named Entity Recognition}},
	Year        = {2020},
	url         = {}
}
```
```
@inproceedings{AQMAR,
 author = {Mohit, Behrang and Schneider, Nathan and Bhowmick, Rishav and Oflazer, Kemal and Smith, Noah A.},
 title = {Recall-oriented Learning of Named Entities in Arabic Wikipedia},
 booktitle = {EACL},
 series = {EACL '12},
 year = {2012},
 isbn = {978-1-937284-19-0},
 location = {Avignon, France},
 pages = {162--173},
 numpages = {12},
 url = {http://dl.acm.org/citation.cfm?id=2380816.2380839},
 acmid = {2380839},
 publisher = {ACL},
 address = {Stroudsburg, PA, USA},
} 
```
