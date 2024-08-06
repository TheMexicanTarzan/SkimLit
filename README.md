# SkimLit: Making Medical Abstracts Skimmable

## Overview

SkimLit is a Recurrent Neural Network (RNN) built with TensorFlow that aims to enhance the readability of medical paper abstracts. By automatically classifying sentences within an abstract into their respective roles (e.g., background, objective, methods, results, conclusions), SkimLit makes scientific literature more accessible and easier to skim.

## Features

- Utilizes state-of-the-art NLP techniques to process medical abstracts
- Classifies sentences into standard abstract sections
- Improves readability and quick comprehension of scientific papers
- Built on TensorFlow for efficient training and inference

## How It Works

SkimLit employs a sophisticated RNN architecture to analyze the content and context of each sentence within a medical abstract. The model has been trained on a dataset by Cornell University (from the paper  "PubMed 200k RCT: a Dataset for Sequenctial Sentence Classification in Medical Abstracts") of pre-labeled abstracts to recognize patterns and features associated with different parts of a scientific abstract. You can find the original paper here: https://arxiv.org/abs/1710.06071

## Usage

To use SkimLit, simply provide the text of a medical abstract:

```python
from skimlit import SkimLit

model = SkimLit()
structured_abstract = model.process_abstract(abstract_text)
print(structured_abstract)
```

The output will be a structured version of the abstract with each sentence labeled according to its role.

## Requirements

- TensorFlow 2.x
- Python 3.7+
- NumPy
- Pandas
  
(Repo in process)
