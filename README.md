# M2FL-CCC

## Introduction

**Gas sensor drift, which has the characteristics of randomness and nonlinearity, is an inevitable problem in electronic nose (E-nose) systems. In this study, a domain-adaptive deep neural network (DNN) framework, called M2FL-CCC, is proposed to suppress sensor drift and improve E-nose performance. This framework mainly contains two key parts: multibranch multilayer feature learning (M2FL) and a comprehensive classification criterion (CCC). In terms of the network structure, a multibranch multilayer structure is designed for customized and joint sensor feature extraction. To fuse the full features of different levels in the network, a joint training strategy is leveraged for multilayer classifiers. Regarding the classification strategy design, a CCC is proposed to fuse the prediction results of the base classifiers and the separation degree between a specific target sample and the source samples. In addition, to optimize the training process, we adopt an improved additional margin softmax classifier with nonlinear dynamic parameter adjustment. Experiments are conducted on public E-nose drift data, and the results show that the M2FL-CCC framework is superior to other compared methods.**

![M2FL-CCC framework](assets\all​.png)


## Quick start for gas detection

```
python3 exe_E_nose_NN.py
```


## Software Structure

- ```exe_E_nose_NN.py```: Entry
- ```utils_data.py```: Store methods for data import and processing
- ```utils_MMD.py```: Store methods related to MMD calculations
- ```utils_network.py```: Store methods related to network structure
- ```./h5```: Store model files
- ```./datasets```: Store dataset files

## Hardware Structure

- Gas sensor array
- Signal conditioning circuit
- Valve control system

![M2FL-CCC hardware](assets\all_hard.png)


## Datasets

- Dataset A: 10 boards, Ref: *Chemical gas sensor drift compensation using classifier ensembles*
- Dataset B: 4 months, Ref: *Online Drift Compensation by Adaptive Active Learning on Mixed Kernel for Electronic Noses*

## Package

- Python 3.7
- Tensorflow 2.4.0
- NumPy 1.19.5




