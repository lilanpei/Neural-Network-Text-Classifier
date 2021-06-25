# Neural Network Text Classifier
We explore a few variants of NN classifiers using word embeddings:
<ul>
<li>Perceptron with One-hot vectors</li>
<li>Perceptron with embeddings</li>
<li>Perceptron with pretrained embeddings</li>
<li>Multilayer perceptron with pretrained embeddings</li>
</ul>
Adapted from code at https://github.com/fchollet/keras/blob/master/examples/imdb_cnn.py

## Import modules
### Set parameters

## Loading data

We will use the `Movie Review dataset` from https://www.kaggle.com/pankrzysiu/keras-imdb.
It contains 50,000 highly polarized reviews, preprocessed, tokenized, indexed and stored into numpy arrays.

By convention, index 0 is reserved for padding, hence set `index_from=1`.
### Split train data into train and validation.

## Perceptron with one-hot representations

*Build a NN binary classifier in Keras using the following layers:*
1. one-hot input representation
4. Dense

*and a cross-entropy loss function.
You may use pretrained GLoVE embeddings from:*
http://medialab.di.unipi.it/jupyterhub/notebooks/HLT/data/glove.6B/glove.first-100k.6B.50d.txt

## Compile the model
`Keras` is built on top `TensorFlow`. Tensorflow allows you to define a computation graph in `Python`, which is then compiled and run efficiently on the CPU or GPU without the overhead of the Python interpreter.

The `compile` method takes three arguments:
- A loss function. The objective that the model will try to minimize. It can be the name of an existing loss function (such as `categorical_crossentropy` or ` mse`), or it can be an objective function.
- An optimizer. The name of an existing optimizer (such as `rmsprop` or `adagrad`), or an instance of the Optimizer class.
- A list of metrics. For any classification problem you will want to set this to `metrics=['accuracy']`. A metric could be the name of an existing metric or a custom metric function.

### Show model
### Train the model
### Evaluate
## Perceptron with Embeddings
### Show the model
### Training
### Testing
### Evaluation
## Exploring the fine-tuned embeddings
### Evaluation
### Explore
## Perceptron with pretrained embeddings
### Perceptron Model
### Train the model
### Evaluate
## Convolutional Neural Network
### Train the model
### Evaluate
