# mucca-dataset
Dataset used in the Mucca paper. You can read the paper [here](https://www.dalsat.me/download/publications/Bacc2012a.pdf).


The dataset itself is in the `data/` directory, which contains three entries:

`mucca-dataset.json`

the full dataset in json format, containing the emails with reference to the original mailing lists, the original raw text, and the classified sentences.


`mucca-dataset-pretty.json`

a pretty-printed copy of mucca-dataset.json


`mucca-dataset.csv`

a list of the classified sentences, with reference to the original email. Each line contains, in this order, the fields:
* `id` - a unique progressive id of the sentence
* `email_id` - the reference to the id of the email
* `classification` - the manual classification of the sentence. The possible values are: _text_, _signature_, _junk_, _link_, _stacktrace_, _code_, _patch_
* `sentence`

The _Jupyter Notebook_ contains the operations to generate the csv from the json, should you need to costomize your dataset.

Citing the dataset
---

If you use this dataset, please cite it using the reference:

```
@inproceedings{Bacc2012a,
	Author = {Bacchelli, Alberto and Dal Sasso, Tommaso and D'Ambros, Marco and Lanza, Michele},
	Booktitle = {In Proceedings of ICSE 2012 (34th ACM/IEEE International Conference on Software Engineering)},
	Keywords = {pub-iene, proj-sosya},
	Pages = {375--385},
	Title = {Content Classification of Development Emails},
	Year = {2012}}
```