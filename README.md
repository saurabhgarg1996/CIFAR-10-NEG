# CIFAR-10-NEG

This repository contains the CIFAR-10-Neg dataset. 

The files CIFAR10_neg.npz contains 1000 datapoints from CINIC-10 test set. This file contains the following keys:

data: an 1000x32x32x10 numpy uint8 array containing the image data   
labels: a numpy int64 array containing labels (integers between 0 and 9)  

``` python
import numpy as np


CIFAR_10_neg = np.load('CIFAR10_neg.npz')

labels = CIFAR_10_neg['labels']
imgs = CIFAR_10_neg['data']

```

We also release the indices of the CINIC-10 test set that we include to create CIFAR-10-Neg in CIFAR10_neg_idx.npz file. Refer to the ipynb for more instruction on how to load the dataset. 
