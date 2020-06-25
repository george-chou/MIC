# MIC
Medical Image Computing Module Development

[![license](https://img.shields.io/github/license/george-chou/MIC.svg)](https://github.com/george-chou/MIC/blob/master/LICENSE)
[![Python application](https://github.com/george-chou/MIC/workflows/Python%20application/badge.svg)](https://github.com/george-chou/MIC/actions)

## Medical Image Enhancement (MIE) ##

The source code of MIE is in `MedicalImageEnhancement.py`

<b>Table 1</b> shows the comparison of the three filters including smoothing, sharpening, edge detection in the aspects of kernel, experiment demo and time cost of running. The way of achieving filter is to use kernel to perform convolution operation on 3D images.

<div align=center>
    <b>Table 1: Comparison of different filters</b>
    <img width="455" src=".github/t1.PNG"/>
</div>

## Medical Image Segmentation (MIS) ##

The source code of MIS is in `MedicalImageSegmentation.py`

<b>Figure 1</b> shows the demonstration of 3D segmentation result achieved using three
multiple viewing angles.

<div align=center>
    <b>Figure 1: 3D segmentation result of the tumor</b>
    <img width="100%" src=".github/f1.png"/>
</div>

<b>Table 2</b> shows the demonstration of the experiments on different global and local parameters combinations. 

<div align=center>
    <b>Table 2: Part experiments on different global and local parameters</b>
    <img width="455" src=".github/t2.PNG"/>
</div>

Based on experiment results, the best global and local parameters are among experiments with ID from 2 to 3 considering the classification of true or false, positive or negative. The best way to find them is to define an indicator of the best result, then define a distance between the result indicator in current parameters and the best result, and finally search for the parameters of minimum distance by deep learning. In that way, we do not need to search for best parameters manually. 