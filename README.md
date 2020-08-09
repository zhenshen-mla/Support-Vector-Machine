# Support-Vector-Machine
SVM有三宝，间隔、对偶、核技巧  
定义：在特征空间上的间隔最大的线性分类器，即求解能够正确划分训练数据集并且几何间隔最大的分离超平面。  
区别于感知机：对于线性可分的数据集来说，感知机划分的超平面有无穷多个，但是几何间隔最大的分离超平面却是唯一的
  
## 推导  
 <div align=left><img width="600" height="700" src="https://github.com/zhenshen-mla/Support-Vector-Machine/blob/master/examples/1.jpg"/></div>  
 <div align=left><img width="600" height="700" src="https://github.com/zhenshen-mla/Support-Vector-Machine/blob/master/examples/2.jpg"/></div>  
 <div align=left><img width="500" height="600" src="https://github.com/zhenshen-mla/Support-Vector-Machine/blob/master/examples/3.jpg"/></div>  
 <div align=left><img width="500" height="600" src="https://github.com/zhenshen-mla/Support-Vector-Machine/blob/master/examples/4.jpg"/></div>  
 <div align=left><img width="500" height="600" src="https://github.com/zhenshen-mla/Support-Vector-Machine/blob/master/examples/5.jpg"/></div>  
 <div align=left><img width="500" height="600" src="https://github.com/zhenshen-mla/Support-Vector-Machine/blob/master/examples/6.jpg"/></div>  

## Files
  * `/data/train.txt & val.txt`: index of train samples and test samples;
  * `/examples/`: examples of train sample, ground truth and prediction;   
  * `/preprocessing/rgb2anno.py`: three-channel label converted to a single channel;   
  * `/utils/loss.py`: loss function for CNNs model;   
  * `/utils/lr_scheduler.py`: learning rate scheduler;
  * `/utils/metrics.py`: evaluation criteria of semantic segmentation;   
  * `/segmentation_model.py`: DeepLabv3 plus structure;
  * `/train_seg.py & test_seg.py`: model testing and training;
  * `/interaction.py`: the front-end interface;
  
## Requirements  

  Python >= 3.0  
  PyTorch >= 1.0  
  numpy  
  torchvision  
  tensorboardX  
  PyQt5  
  PyInstaller  
  

## Installation
  1. Clone the repo:   
    ```
    git clone https://github.com/zhenshen-mla/Satellite-Image-Segmentation.git   
    ```   
    ```
    cd Satellite-Image-Segmentation   
    ```
  2. For custom dependencies:   
    ```
    pip install tensorboardX matplotlib PyQt5 PyInstaller   
    ```

## Running
  1. Model training:   
    ```
    python train_seg.py   
    ```   
  2. Model testing:   
    ```
    python test_seg.py   
    ```
  3. Package model and front-end interaction:   
    ```
    pyinstaller -F interaction.py   
    ```

