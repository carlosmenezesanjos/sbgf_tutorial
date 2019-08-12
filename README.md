# SBGF enviroment preparation instructions
This is an installation instructions guide for the enviroment used on SBGF Machine Learning and Deep Learning Tutorial.

# CUDA and CUDNN

If you have on your machine a nvidia gpu that supports cuda 10.0 the first step is to install cuda 10.0 and cudnn >= 7.4.1. If you don't  skip to the enviroment creation.

Guides that will help you with cuda installation:

[https://www.tensorflow.org/install/gpu](https://www.tensorflow.org/install/gpu)
[https://docs.nvidia.com/cuda/index.html](https://docs.nvidia.com/cuda/index.html)
[https://docs.nvidia.com/deeplearning/sdk/cudnn-install/index.html](https://docs.nvidia.com/deeplearning/sdk/cudnn-install/index.html)

# Enviroment creation with Anaconda

1. Download Anaconda for your operational system [https://www.anaconda.com/distribution/](https://www.anaconda.com/distribution/) and follow it's installation guide [https://docs.anaconda.com/anaconda/install/](https://docs.anaconda.com/anaconda/install/)
2. Download the requirements.txt that is available on this repository.
    If you have a nvidia gpu and already installed cuda and cudnn, download the requirements.txt available on ./gpu/requirements.txt
    If you don't have a nvidia gpu, download the requirements.txt available on ./cpu/requirements.txt

Now there are two options to create the enviroment one via terminal and the other using Anaconda Navigator.

Via terminal:
1. Open the terminal on the folder with the requirements.txt file and execute
  ```sh
  conda create -n deep_learning python=3.7
  ```
  ```sh
  pip install -r requirements.txt
  ```
  
Via Anaconda Navigator:
1. Open anaconda navigator, clicking it's icon or via terminal with 
  ```sh
  anaconda-navigator
  ```
2. On the tab enviroments, click the button create to create a new enviroment.
![](../createbutton.png)
3. Fill the fields with name and package and click the button to create, this may take a few minutes.
![](../createbuttonoptions.png)
4. Once created, to activate the enviroment, select the enviroment by click over it's name and on the play symbol. This will open an options window, select open terminal.
5. On terminal, navigate to the folder where the requirements.txt is located and execute
  ```sh
  pip install -r requirements.txt
  ```
  


