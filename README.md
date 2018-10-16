# Deep Learning On 2-Dimentional Images

## 1. What is 2-Dimentional image ? 
One type of picture you can come across in real life is the two-dimensional one. The two dimensions depicted are length and width and the objects on the picture are flat.


![picture alt](https://vignette.wikia.nocookie.net/animal-jam-clans-1/images/e/e7/2d.jpg/revision/latest?cb=20160919185703 "Title is optional")



## 2. How to handle these data ?
There are many libraries in Python to handle these kind of data:
  1. Keras (<https://keras.io/>)
  2. Tensorflow (<https://www.tensorflow.org/tutorials/)
  3. cv2 (<https://opencv-python-tutroals.readthedocs.io/en/latest/py_tutorials/py_gui/py_image_display/py_image_display.html>)
  


## 3. How these model work ?

![picture alt](https://www.researchgate.net/publication/314282902/figure/fig1/AS:469481303613440@1488944473917/Architecture-of-the-proposed-CNN-model-with-2-convolutional-layers.png "Title is optional")



Convolutional Neural Network is a neural network consists of convolutional layer, pooling layer (max pooling or average pooling but max pooling is preferable), fully connected layer and at last a softmax pooling

Object_detection.py explains how to create a simple convnet using keras framwork.



## 4. Area of application ?
1. Medical problems
    1. MRI dataset
    2. CT Scan
    3. Xray Scans etc.
    4. InfraRed Images
2. Thermal images
3. Agricultural problems 
4. Satellite images etc



## 4.1 Medical Problems
### 4.1.1 MRI dataset
#### MRI Background

Magnetic Resonance Imaging (MRI) is the most common diagnostic tool brain tumors due primarily to it's noninvasive nature and ability to image diverse tissue types and physiological processes. MRI uses a magnetic gradient and radio frequency pulses to take repetitive axial slices of the brain and construct a 3-dimensional representation(Figure 2). Each brain scan 155 slices, with each pixel representing a 1mm<sup>3</sup> voxel.  

<img alt="Basic MRI Workflow" src="https://github.com/naldeborgh7575/brain_segmentation/raw/master/images/MRI_workflow.png" width=450>
<img alt="3D rendering produced by T2 MRI scan" src="https://github.com/naldeborgh7575/brain_segmentation/raw/master/images/t29_143.gif" width=250>  



#### MRI pre-processing ([code](https://github.com/naldeborgh7575/brain_segmentation/blob/master/code/brain_pipeline.py))

One of the challenges in working with MRI data is dealing with the artifacts produced either by inhomogeneity in the magnetic field or small movements made by the patient during scan time. Oftentimes a bias will be present across the resulting scans (Figure 3), which can effect the segmentation results particularly in the setting of computer-based models.

<img alt="Bias correction before and after" src="https://github.com/naldeborgh7575/brain_segmentation/raw/master/images/n4_correction.png" width=200>  
