# CIFAR-10-NEG

This repository contains the CIFAR-10-Neg dataset prepared and published in "Deconstructing Distributions: A Pointwise Framework of Learning" by Gal Kaplun, Nikhil Ghosh, Saurabh Garg, Boaz Barak, Preetum Nakkiran.

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

If you find this data useful, please cite the following paper: 

> Kalpun, G., Ghosh, N., Garg, S., Boaz, B., Nakkiran, P. (2022). Deconstructing Distributions: A Pointwise Framework of Learning. arxiv preprint arXiv:2202.09931. 
```
@article{kalpun2022deconstructing,
    title={Deconstructing Distributions: A Pointwise Framework of Learning},
    author={Kalpun, Gal and Ghosh, Nikhil and Garg, Saurabh and Barak, Boaz and Nakkiran, Preetum },
    year={2022},
    journal={arXiv preprint arXiv:2202.09931},
}
```

In addition, please consider [citing](https://raw.githubusercontent.com/saurabhgarg1996/CIFAR-10-NEG/main/cinic10_bibtex.txt) the paper accompanying the CINIC-10 data (of which CIFAR-10-Neg is a subset). 
