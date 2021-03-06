# Face-Alignment-with-Two-Stage-Re-initialization
The test code of the CVPR 2017 paper **"A Deep Regression Architecture with Two-Stage Re-initialization for High Performance Facial Landmark Detection"**.

<img src="figures/overflow.jpg" width = "70%" />

## Requirement
  1. General environment for Caffe platform on Linux OS: https://github.com/BVLC/caffe. 
  2. Matlab 2013a or later
  3. Cuda (if use nvidia gpu)

## Introduction
   <img src="figures/diff-det.jpg" width = "50%" />
<br>
Since different face detectors often return various face bounding boxes with different scales and center shifts, it would be very useful if a facial landmark detection algorithm can produce robust results without depending so much on the face detection results. To explicitly deal with the initialization problem in regression based landmark detection methods, we present a deep regression architecture with **two-stage re-initialization** learned from end to end. Our proposed deep architecture is trained from end to end and obtains promising results using different kinds of unstable initialization. It also achieves superior performances over many competing algorithms.    
<br>
     
<br>  
  
The comparison of our method and other baseline methods on 300-W and AFLW dataset are shown as follows, more details can be found in the initial paper.
 <br> 
   <img src="figures/300W-results.jpg" width = "50%" />
   <img src="figures/aflw-results.jpg" width = "50%" />
   
## Run the test code
The models are saved at Baidu SkyDrive: <br>
Model for 300-W: link: http://pan.baidu.com/s/1gfxfv8J password：qzmi   <br>
Model for aflw:  link: http://pan.baidu.com/s/1cEk3Zw password：1j8e <br> 

<br> 
When you had successfully built the CAFFE in this project and downloaded the models, just run the `main_300w_part.m` and `main_aflw_part.m` in the demo folder.
   
  
### Acknowledgement
  The source code of st_layer.cpp and st_layer.cu come from [here](https://github.com/christopher5106/last_caffe_with_stn).
### Citation
```
If you find this work useful, please cite as follows:
  @inproceedings{lv2017twostage,  
  title={A Deep Regression Architecture with Two-Stage Re-initialization for High Performance Facial Landmark Detection},  
  author={Lv, Jiangjing and Shao, Xiaohu and Xing, Junliang and Cheng, Cheng and Zhou, Xi},  
  booktitle={Proceedings of the IEEE conference on computer vision and pattern recognition},  
  year={2017}  
 }
```

### Licence
This code is distributed under MIT LICENSE.

### Contact
Please contact us if you have any problems during the demo running: <br> 

Jiangjing Lv lvjiangjing12 at gmail dot com <br>
Xiaohu Shao shaoxiaohu at cigit dot ac dot cn <br>
Junliang Xing jlxing at nlpr dot ia dot ac dot cn <br>
