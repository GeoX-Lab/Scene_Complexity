# Scene_Complexity
This repo includes the source code for the paper:  
Scene Complexity: A New Perspective on Understanding the Scene Semantics of Remote Sensing and Designing Image-Adaptive Convolutional Neural Networks. Remote Sens. 2021, doi: 10.3390/rs13040742.

## Abstract:
Scene understanding of remote sensing images is of great significance in various applications. Its fundamental problem is how to construct representative features. Various convolutional neural network architectures have been proposed for automatically learning features from images. However, is the current way of configuring the same architecture to learn all the data while ignoring the differences between images the right one? It seems to be contrary to our intuition: it is clear that some images are easier to recognize, and some are harder to recognize. This problem is the gap between the characteristics of the images and the learning features corresponding to specific network structures. Unfortunately, the literature so far lacks an analysis of the two. In this paper, we explore this problem from three aspects: we first build a visual-based evaluation pipeline of scene complexity to characterize the intrinsic differences between images; then, we analyze the relationship between semantic concepts and feature representations, i.e., the scalability and hierarchy of features which the essential elements in CNNs of different architectures, for remote sensing scenes of different
complexity; thirdly, we introduce CAM, a visualization method that explains feature learning within neural networks, to analyze the relationship between scenes with different complexity and semantic feature representations. The experimental results show that a complex scene would need deeper and multi-scale features, whereas a simpler scene would need lower and single-scale features. Besides, the complex scene concept is more dependent on the joint semantic representation of multiple objects. Furthermore, we propose the framework of scene complexity prediction for an image and utilize it to design a depth and scale-adaptive model. It achieves higher performance but with fewer parameters than the original model, demonstrating the potential significance of scene complexity

[!image](https://github.com/GeoX-Lab/Scene_Complexity/blob/main/CAM_master/GA.png)

## Requirement

* Matlab 2012 or later 
* Caffe     

## Data
Basing [AID](www.lmars.whu.edu.cn/xia/AID-project.html), we select 22 categories scene as our dataset,considering its diacritical scene complexity.
                       <div align=center><img src="https://github.com/wzx918/images/blob/master/%E6%8D%95%E8%8E%B71.PNG"/></div>
                       
## Run
This source code is released under an Attribution-NonCommercial 4.0 International license, find more about it [here](https://github.com/GeoX-Lab/ANPyC/blob/main/LICENSE)

## Citation
If our repo is useful to you, please cite our published paper as follow:

```
Bibtex
@article{peng2021scene,
    title={Scene Complexity: A New Perspective on Understanding the Scene Semantics of Remote Sensing and Designing Image-Adaptive Convolutional Neural Networks},
    author={Peng, Jian and Mei, Xiaoming and Li, Wenbo and Hong, Liang and Sun, Bingyu and Li, Haifeng},
    journal={Remote Sens},
    DOI = {10.3390/rs13040742},
    year={2021},
    type = {Journal Article}
}
