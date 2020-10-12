# Predicting the next sentence. 
Deep Learning based Text generation

Input file: melville_moby_dick.txt (This is a large file, you can also download the smaller version: moby_dick_four_chapters.txt)
This notebook describes the process of generating predictive text generation using Keras and LSTM.

## Dependencies
Install the following using pip3 install <pkgName> (optional flag: --user if multiple users on an instance). The package name follows import/from command. e.g. import <pkgName> or from <pkgName> import <function>
import spacy
import numpy as np
import random
from random import randint
from pickle import load

import keras
from keras.preprocessing.text import Tokenizer
from keras.models import load_model, Sequential
from keras.layers import Dense,LSTM,Embedding
from keras.utils import to_categorical

from keras.preprocessing.sequence import pad_sequences
  
## Contributing
Pull requests are welcome. For major changes, please open an issue first to discuss what you would like to change.

## Disclaimer: 
Adapted from my Udemy course project by Jose Portilla.
