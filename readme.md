Can Sparse Representations be Used to Classify and Cluster Small Samples of Satellite Images?

Introduction:
When one thinks of image recognition, deep neural nets and vast data sets come to mind. We are interested in discovering if, using basic techniques from EE290T, small samples of textured images can be clustered and classified in a meaningful way. 

Team Members: 
Ashray Manepalli, Liam Purvis, Shi Mao

The Data:
We are sourcing our data from the kaggle competition Planet, which challenged individuals to classify satellite images of the Amazon into a variety of categories (‘forested’, ‘developed’, ‘agriculture’, ‘cloudy’, ‘hazy’, etc). 

Overview: 
In class, we have covered techniques for recovering vectors such that they satisfy certain ‘sparsity’ based properties. Find the sparsest vector satisfying y = Ax, or the lowest rank data for Y = AX, for some measurement matrices A. 
Here we have data containing textured segments with high redundancy - data that typically has some intrinsic low rank representation. Instead of a ‘recovery’ task, we approach this as a dimensional reduction and feature extraction task. We aim to test and create different measurement and classification techniques that allow us to obtain some regularized low rank but highly representational version of our irregular textured data.

We will choose two or three categories of images from our Satellite Dataset with distinct textural differences (say ‘forested, ‘cloudy’, ‘agriculture’) and then see if the low dimensional representations of these images are distinct enough to classify using traditional (non-neural) techniques on a small dataset. Our goal is to fix our Machine learning analysis, and iterate over our dimensional reductions and sparse representation of these images, so as to better understand how these techniques affect our outcome. 

Steps in Our Process:
Access and curate a dataset with three categories, selecting a test sets, training sets, and validation sets numbering 100, 50, 50 each respectively (for a total of 600 images).

Reduce dimensions of images, exploring structured wavelet transforms, analysis of basis vectors, sparse dictionary learning.

Visualize clusters and predict classes using spectral clustering and traditional small sample machine learning techniques (SVM, random forest, or multivariate gaussian models).

Analysis of most effective dimensional reductions for clustering and classification of small samples of images with different patterns/texture in this real world application. 

Tools:
The final submission will be a jupyter notebook, but we will likely be working collaboratively on a python file using git. 
Our IDE will be Atom, with the hydrogen extension to simulate the cells of a notebook.
Pytorch, for Neural Networks, Scattering Networks
Sklearn for other machine learning algorithms.
Wavelets and signal processing packages: pywt, skimage, 

Algorithms:
DIMENSIONAL REDUCTION:
Wavelets
Dictionary learning
PCA
Finding basis vectors
Filter bank methods
UNSUPERVISED LEARNING:
Spectral Analysis
SUPERVISED LEARNING:
Neural Networks
Multivariate Gaussian
SVM.


Papers and writings we will be using as reference:
https://arxiv.org/pdf/1312.5940.pdf
http://www.mipg.upenn.edu/yubing/2005ICMLC.pdf
https://www.sciencedirect.com/science/article/pii/S0262885603000945
https://www.sciencedirect.com/science/article/pii/S016516840500277X#fig3
http://mcl.usc.edu/wp-content/uploads/2014/01/1993-10-Texture-analysis-and-classification-with-tree-structured-wavelet-transform.pdf

Github:
https://github.com/Sheldonmao/290texture

