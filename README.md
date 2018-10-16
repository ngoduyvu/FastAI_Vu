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
The move 37 is a deep learning code create by Siraj RaVal
