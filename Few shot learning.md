# Few shot learning

## 1. Understanding few-shot learning in machine learning
https://medium.com/quick-code/understanding-few-shot-learning-in-machine-learning-bede251a0f67

### What is few-shot learning?
few-shot learning refers to the practice of feeding a learning model with a very small amount of training data, 
contrary to the normal practice of using a large amount of data.

Example:
For example, if we have a problem of categorizing bird species from photos, 
some rare species of birds may lack enough pictures to be used in the training images.

Consequently, if we have a classifier for bird images, with the insufficient amount of the dataset, 
we’ll treat it as a few-shot or low-shot machine learning problem.

If we have only one image of a bird, this would be a one-shot machine learning problem. 
In extreme cases, where we do not have every class label in the training, and we end up with 0 training samples in some categories, 
it would be a zero-shot machine learning problem.

### Motivations for few-shot machine learning

* Whenever there is scarcity of supervised data, machine learning models often fail to carry out reliable generalizations.
* When working with a huge dataset, correctly labeling the data can be costly.
* When several samples are available, adding specific features for every task is strenuous and difficult to implement.

### Low-shot learning approaches
####  Data-level approach
- A common technique used to realize this is to tap into an extensive collection of external data sources. 
For example, if the intention is to create a classifier for the species of birds without sufficient labeled elements for each category, 
it could be necessary to look into other external data sources that have images of birds.
- In addition to utilizing external data sources, another technique for data-based low-shot learning is to produce new data: data augmentation or GAN

#### Parameter-level approach
* regularization techniques or loss functions are often employed

## 2. Transfer Learning — part 2
https://medium.com/dataswati-garage/transfer-learning-part-2-zero-one-few-shot-learning-8d23d2f8583b
