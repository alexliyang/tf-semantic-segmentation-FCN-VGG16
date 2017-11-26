# Semantic Segmentation
[![Udacity - Self-Driving Car NanoDegree](https://s3.amazonaws.com/udacity-sdc/github/shield-carnd.svg)](http://www.udacity.com/drive)

- This repository is for udacity self-driving car nanodegree project: `Semantic Segmentation`.
- Implement this paper: ["Fully Convolutional Networks for Semantic Segmentation (2015) "](https://people.eecs.berkeley.edu/~jonlong/long_shelhamer_fcn.pdf)
- See [`FCN-VGG16.ipynb`](./FCN-VGG16.ipynb)


## Implementation Details
### Network
- `FCN8s` with `VGG16` as below figure.
![network figure](https://devblogs.nvidia.com/parallelforall/wp-content/uploads/2016/11/figure15.png)

### Dataset
- [Kitti Road dataset](http://www.cvlibs.net/datasets/kitti/eval_road.php) from [here](http://www.cvlibs.net/download.php?file=data_road.zip).

### Hyperparameters
- Optimizer: AdamOptimizer
- Learning rate: 1e-3
- Deconvolution `l2` regularization factor: 1e-3
- Batch size: 16
- Training Epochs: 50

## Results
### Optimization
- After 50 epochs, loss became about 0.1
![loss](./assets/loss.png)

### Nice results
- These are pretty nice results. it looks that network can classify road well.
![good1](./assets/good1.png)
![good2](./assets/good2.png)
![good3](./assets/good3.png)
![good4](./assets/good4.png)
![good5](./assets/good5.png)
![good6](./assets/good6.png)
![good7](./assets/good7.png)
![good8](./assets/good8.png)


### Bad results
- These are bad results. I believe this could be better after following methods:
  - Use more deeper network (e.g. ResNet)
  - Augment given data or use another data (e.g. CityScape)

![bad1](./assets/bad1.png)
![bad2](./assets/bad2.png)
![bad3](./assets/bad3.png)
![bad4](./assets/bad4.png)


---

### Setup
##### Frameworks and Packages
Make sure you have the following is installed:
 - [Python 3](https://www.python.org/)
 - [TensorFlow](https://www.tensorflow.org/)
 - [NumPy](http://www.numpy.org/)
 - [SciPy](https://www.scipy.org/)

### Start
##### Implement
Implement the code in the `main.py` module indicated by the "TODO" comments.
The comments indicated with "OPTIONAL" tag are not required to complete.
##### Run
Run the following command to run the project:
```
python main.py
```
**Note** If running this in Jupyter Notebook system messages, such as those regarding test status, may appear in the terminal rather than the notebook.

### Submission
1. Ensure you've passed all the unit tests.
2. Ensure you pass all points on [the rubric](https://review.udacity.com/#!/rubrics/989/view).
3. Submit the following in a zip file.
 - `helper.py`
 - `main.py`
 - `project_tests.py`
 - Newest inference images from `runs` folder  (**all images from the most recent run**)

 ## How to write a README
A well written README file can enhance your project and portfolio.  Develop your abilities to create professional README files by completing [this free course](https://www.udacity.com/course/writing-readmes--ud777).
