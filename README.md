<div style="background-color: #F0ECE1; padding: 10px; border-radius: 5px;">
    <div style="margin-bottom: 10px; text-align: center;">
        <h1 style="color: #3C3530; font-size: 36px; font-weight: bold; margin-bottom: 10px;">
            A Natural Look into our AI-Driven World: An Image Classification Lookthrough
        </h1>
    </div>
</div>

<img src="https://images.pexels.com/photos/869258/pexels-photo-869258.jpeg?auto=compress&cs=tinysrgb&w=1260&h=750&dpr=1">

TL;DR
This image classification project identifies settings and categories of images automatically from Intel's natural world dataset.
Our method utilizes Tensorflow on Python 3 to execute a classification process with a model accuracy of 74.8%. Not bad, but this suggests that there are opportunities for improvement. 
The loss in the test sets that is affecting accuracy comes down to Glacier and Sea images.

AI is changing the world as we know it. Companies look to train models based on recurring patterns, and visuals such as images make for great training material to help them identify and improve upon their ability to predict patterns and accuracy. 
For this project, we will be using Tensorflow. Tensorflow is an ML package from Google that enables analysts and engineers to develop everything from Simple Neural Networks to Image Classification. 
We're gonna focus on the latter, so this project will concentrate on using Keras.

The dataset used: https://www.kaggle.com/datasets/puneet6060/intel-image-classification

## Installation
I highly recommend using [VS Code](https://code.visualstudio.com/) to manage your python environment. 
From there, install Tensorflow by first installing Miniconda and then Tensorflow. Full instructions can be found [here](https://www.tensorflow.org/install/pip#macos_1)

I used the following for my Macbook Pro M1 Max laptop (Apple Silicon) machine:
```
#Miniconda
curl https://repo.anaconda.com/miniconda/Miniconda3-latest-MacOSX-x86_64.sh -o Miniconda3-latest-MacOSX-x86_64.sh
bash Miniconda3-latest-MacOSX-x86_64.sh

#Conda activation
conda create --name tf python=3.9
conda conda activate tf

#Pip Upgrade
pip install --upgrade pip

#Pip Install
pip install tensorflow

#Verify
python3 -c "import tensorflow as tf; print(tf.reduce_sum(tf.random.normal([1000, 1000])))"
```
