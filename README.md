[![fastai python compatibility](https://img.shields.io/pypi/pyversions/fastai.svg)](https://pypi.python.org/pypi/fastai)

# FastAI Course
**Setup locally**
* Step 1: Install Conda
Anaconda is a develop environment which is very popular in Python developer and Data Scienst communities. The environment can be download from [conda's website](https://www.anaconda.com/download/), the Linux operation can install Anaconda by following command. 
```
pip install conda
```
* Step 2: Set Up GPU Operation For Pytorch
```
conda install -c pytorch-nightly cuda92
conda install -c fastai torchvision-nightly
conda install -c fastai fastai 
```
* Step 3: Update all package to the lastest version
```
conda update conda
conda search --outdate
conda update --all
```
* Step 4: 
```
gitclone https://github.com/fastai/fastai
cd fastai
tools/run-after-git-clone
pip install -e .[dev]
```
**Setup on Cloud**
The FastAI environment can be setup on AWS EC2, AWS maketplace provide pre-build Amazon instance called "Deep Learning AMI (Ubuntu)" which provides all popular deep learning frameworks such as Tensorflow, Pytorch, Caffe, Apache MXNet. The size of Amazon instance should be around "t2.xlarge", the cost for Amazon is quite expensive.

The Kaggle provides free kernel to run FastAI lession, all the notebook are provided data with neccessary GPU power. 
the lession 4 of Kaggle's kernel has some error but the remain is fine. <br/> 
Lession 1: https://www.kaggle.com/hortonhearsafoo/fast-ai-lesson-1 <br/>
Lession 2: https://www.kaggle.com/hortonhearsafoo/fast-ai-lesson-2 <br/>
Lession 3: https://www.kaggle.com/hortonhearsafoo/fast-ai-lesson-3 <br/>
Lession 4: https://www.kaggle.com/hortonhearsafoo/fast-ai-lesson-4 <br/>
Lession 5: https://www.kaggle.com/hortonhearsafoo/fast-ai-lesson-5 <br/>
Lession 6a: https://www.kaggle.com/hortonhearsafoo/fast-ai-lesson-6-sgd <br/>
Lession 6b: https://www.kaggle.com/hortonhearsafoo/fast-ai-lesson-6-rnn <br/>
Lession 7a: https://www.kaggle.com/hortonhearsafoo/fast-ai-lesson-7-cifar10 <br/>
Lession 7b: https://www.kaggle.com/hortonhearsafoo/fast-ai-lesson-7-cam <br/>

Summary FastAI Course:<br> 
https://medium.com/@hiromi_suenaga<br>
https://www.kdnuggets.com/2018/07/fast-ai-deep-learning-part-1-notes.html<br>


# Move 37
The move 37 is a deep learning code create by Siraj RaVal, the code teach about Reinforment Learning and several new technology in Deel Learning technology.

![RL](https://github.com/ngoduyvu/FastAI_Vu/blob/master/SchoolAI/Img/Deep%20Reinforcement%20Learning.png) 
###### Source: CS 294 Deep Reinforcement Learning (UC Berkeley)

Reinforcement Learning (RL) is a type of Machine Learning, it automatically determine an ideal behavious within a specific enviroment or context in order to maximize its performance.The RL models find the optimal behaviors by choose actions which return the most rewards based on feedback from the environment. RL differs from normal supervised machine learning models in that correct input/output pairs need not be presented, and sub-optimal actions need not be explicitly corrected.Instead the focus is on performance , which involves finding a balance between exploration (of uncharted territory) and exploitation (of current knowledge).

## Tips for improving Deep Learning model
1. Data Optimization
One of the easiest ways to increase performance for underperforming deep learning models is to balance your dataset if your problem is classification. Often real-world data sets are skewed, there are a few tricks which could help deep learning model to due with unbalance data.
  * Subsample Majority Class: You can balance the class distributions by subsampling the majority class.
  * Oversample Minority Class: Sampling with replacement can be used to increase your minority class proportion.
  * Add or Generate More Data: Find similar data to add to the existing data or use machine learning model create new data.
2. Algorithm tuning
  * Use the same algorithms which researchers used for similar problems
  * Try different models for a same problem.
3. Hyper-Parameter Optimization
  * Learning rates: A standard procedure is using large batch sizes with a large number of epochs for modern deep learning implementations, but common strategies yield common results. Experiment with the size of your batches and the number of training epochs.
  * Batch size and number of epochs: A standard procedure is using large batch sizes with a large number of epochs for modern deep learning implementations, but common strategies yield common results. Experiment with the size of your batches and the number of training epochs.
  * Early Stopping: This is an excellent method for reducing the generalization error of your deep learning system. Continual training might improve accuracy on your data set, but at a certain point, it starts to reduce the model’s accuracy on data not yet seen by the model. To improve real-world performance try early stopping.
  * Network Architecture: By exploring different architecture of a same types of a Deep Learning Model, you can find the optimize architecture. 
  * Regularization: A robust method to stop overfitting is to use regularization. There are a couple of different ways to use regularization that you can train on your deep learning project. If you haven’t tried these methods yet I would start to include them into every project you do. 
4. Ensembles
You can combine the outputs from the different models and get better accuracy. There are two steps for every one of these algorithms.
  * Producing a distribution of simple ML models on subsets of the original data
  * Combining the distribution into one “Aggregated” model
  

