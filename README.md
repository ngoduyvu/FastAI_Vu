

# FastAI_Vu
Set up locally
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

Run FastAI lession on Kaggle:
Lession 1: https://www.kaggle.com/hortonhearsafoo/fast-ai-lesson-1 <br/>
Lession 2: https://www.kaggle.com/hortonhearsafoo/fast-ai-lesson-2 <br/>
Lession 3: https://www.kaggle.com/hortonhearsafoo/fast-ai-lesson-3 <br/>
Lession 4: https://www.kaggle.com/hortonhearsafoo/fast-ai-lesson-4 <br/>
Lession 5: https://www.kaggle.com/hortonhearsafoo/fast-ai-lesson-5 <br/>
Lession 6a: https://www.kaggle.com/hortonhearsafoo/fast-ai-lesson-6-sgd <br/>
Lession 6b: https://www.kaggle.com/hortonhearsafoo/fast-ai-lesson-6-rnn <br/>
Lession 7a: https://www.kaggle.com/hortonhearsafoo/fast-ai-lesson-7-cifar10 <br/>
Lession 7b: https://www.kaggle.com/hortonhearsafoo/fast-ai-lesson-7-cam <br/>

Summary FastAI Course: 
https://medium.com/@hiromi_suenaga/deep-learning-2-part-1-lesson-1-602f73869197<br>
https://www.kdnuggets.com/2018/07/fast-ai-deep-learning-part-1-notes.html<br>
