# Bengali GloVe Word Vectors

* [Bengali Pretrained Vectors](#download-bengali-pre-trained-word-vectors)

## GloVe: Global Vectors for Word Representation


| nearest neighbors of <br/> <em>frog</em> | Litoria             |  Leptodactylidae | Rana | Eleutherodactylus |
| --- | ------------------------------- | ------------------- | ---------------- | ------------------- |
| Pictures | <img src="http://nlp.stanford.edu/projects/glove/images/litoria.jpg"></img> | <img src="http://nlp.stanford.edu/projects/glove/images/leptodactylidae.jpg"></img> | <img src="http://nlp.stanford.edu/projects/glove/images/rana.jpg"></img> | <img src="http://nlp.stanford.edu/projects/glove/images/eleutherodactylus.jpg"></img> |

| Comparisons | man -> woman             |  city -> zip | comparative -> superlative |
| --- | ------------------------|-------------------------|-------------------------|
| GloVe Geometry | <img src="http://nlp.stanford.edu/projects/glove/images/man_woman_small.jpg"></img>  | <img src="http://nlp.stanford.edu/projects/glove/images/city_zip_small.jpg"></img> | <img src="http://nlp.stanford.edu/projects/glove/images/comparative_superlative_small.jpg"></img> |

We provide an implementation of the GloVe model for learning word representations, and describe how to download web-dataset vectors or train your own. See the [project page](http://nlp.stanford.edu/projects/glove/) or the [paper](http://nlp.stanford.edu/pubs/glove.pdf) for more information on glove vectors.

## Download Bengali pre-trained word vectors

NB: We evaluated this trained vectors with `common-countries-bn.txt & family-bn.txt`(inside eval/question-data-bn) question data. and Accuracy is 34%</br>
In next version we will create a better question data for evaluation and will publish final evaluation result.

* wikipedia+crawl_news_articles (39M(39055685) tokens, 0.18M(178152) vocab size, 195.4MB download):</br> [bn_glove.39M.300d.zip](https://drive.google.com/open?id=1TugAM1l-hIIR2foW8KhckfCyMNfdmzCY)

* wikipeida+crawl_news_articles (39M(39055685) tokens, 0.18M(178152) vocab size, 100d vectors, 65MB download):</br> [bn_glove.39M.100d.zip](https://drive.google.com/open?id=1HJYOg3kEMVIrJ013Q8MeG0hRnMI3jxYx)

* Wikipedia (20M(19965328) tokens, 0.13M(134255) vocab, 300d vectors, 145.9MB download):</br> [bn_glove.300d.zip](https://drive.google.com/open?id=1o6wBjaRX8fUOZfqSAVA3TSBBNVVvk3nt)

* Wikipedia (20M(19965328) tokens, 0.13M(134255), 100d vectors, 51.2MB download):</br> [bn_glove.100d.zip](https://drive.google.com/open?id=1in1MbQXieuvytsqIP9Q8qFgnTSZEHMue)

## Dataset
* [wikipedia](https://dumps.wikimedia.org/bnwiki/latest/)


## Play With Pretrained Vectors

```python test.py```


## Train word vectors on a new corpus

<img src="https://travis-ci.org/stanfordnlp/GloVe.svg?branch=master"></img>

If the web datasets above don't match the semantics of your end use case, you can train word vectors on your own corpus.

    $ git clone http://github.com/stanfordnlp/glove
    $ cd glove && make
    $ ./demo.sh

The demo.sh script downloads a small corpus, consisting of the first 100M characters of Wikipedia. It collects unigram counts, constructs and shuffles cooccurrence data, and trains a simple version of the GloVe model. It also runs a word analogy evaluation script in python to verify word vector quality. More details about training on your own corpus can be found by reading [demo.sh](https://github.com/stanfordnlp/GloVe/blob/master/demo.sh) or the [src/README.md](https://github.com/stanfordnlp/GloVe/tree/master/src)

## Evaluation

```
python eval/python/evaluate.py \
--vocab_file /path/vocab.txt
--vectors_file /path/vectors.txt
```

### License
All work contained in this package is licensed under the Apache License, Version 2.0. See the include LICENSE file.

# Contributor
[![](https://sourcerer.io/fame/sagorbrur/sagorbrur/GloVe-Bengali/images/0)](https://sourcerer.io/fame/sagorbrur/sagorbrur/GloVe-Bengali/links/0)[![](https://sourcerer.io/fame/sagorbrur/sagorbrur/GloVe-Bengali/images/1)](https://sourcerer.io/fame/sagorbrur/sagorbrur/GloVe-Bengali/links/1)[![](https://sourcerer.io/fame/sagorbrur/sagorbrur/GloVe-Bengali/images/2)](https://sourcerer.io/fame/sagorbrur/sagorbrur/GloVe-Bengali/links/2)[![](https://sourcerer.io/fame/sagorbrur/sagorbrur/GloVe-Bengali/images/3)](https://sourcerer.io/fame/sagorbrur/sagorbrur/GloVe-Bengali/links/3)[![](https://sourcerer.io/fame/sagorbrur/sagorbrur/GloVe-Bengali/images/4)](https://sourcerer.io/fame/sagorbrur/sagorbrur/GloVe-Bengali/links/4)[![](https://sourcerer.io/fame/sagorbrur/sagorbrur/GloVe-Bengali/images/5)](https://sourcerer.io/fame/sagorbrur/sagorbrur/GloVe-Bengali/links/5)[![](https://sourcerer.io/fame/sagorbrur/sagorbrur/GloVe-Bengali/images/6)](https://sourcerer.io/fame/sagorbrur/sagorbrur/GloVe-Bengali/links/6)[![](https://sourcerer.io/fame/sagorbrur/sagorbrur/GloVe-Bengali/images/7)](https://sourcerer.io/fame/sagorbrur/sagorbrur/GloVe-Bengali/links/7)
