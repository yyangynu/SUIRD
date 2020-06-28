These mat files provide the raw data of the image pair and groundTruth data

1) raw data(Num.mat)
tip: In python, mat file can be read using code mat = scipy.io.loadmat(mat_path)

image1: The sensed image data, it is stored as a height*width*3 matrix. Python code: img_s = mat['image1']
image2: The reference image data, it is stored as a height*width*3 matrix, Python code: img_r = mat['image2']
point1: The coordinates of SIFT points, it is stored as a n*2 matrix. Python code: pre_s = mat['point1']
point2: The coordinates of SIFT points, it is stored as a n*2 matrix. Python code: pre_r = mat['point2']
*: pre_s[i] and pre_r[i] is the initial correspondence (prematches), where i = 1, 2, 3, ...... n

2) Groundtruth data(Num-Completed.mat)
tip: In python, mat file can be read using code mat = scipy.io.loadmat(mat_path)
The groundtruth is determined manually, 1 represents the correct correspondence (inlier) and 0 represents incorrect correspondence (outlier) ,it is stored as a n*1 matrix. Python code: ground_true = mat['GroundTruth']

-----------------------------------------------------------------------
This document was last modified on : 6.26 2020.
Copyright (C) 2020, Yang Yang.