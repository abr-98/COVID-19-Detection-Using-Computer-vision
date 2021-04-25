# COVID-19-Detection-Using-Computer-vision
Application of Transfer learning and Deep Feature Extraction Networks to detect COVID-19 from Chest-CT Scans and Chest-X_rays

Dataset Used: https://github.com/abr-98/COVID_dataset

Reference Papers: 
1. https://doi.org/10.1016/j.bspc.2021.102588  ## Architecture Adaptation
2. https://doi.org/10.1016/j.imu.2020.100360   ## Architecture Adaptation
3. https://www.nature.com/articles/s41598-020-76550-z
4. https://link.springer.com/article/10.1007/s00330-021-07715-1
5. https://openaccess.thecvf.com/content_cvpr_2017/papers/Lin_Feature_Pyramid_Networks_CVPR_2017_paper.pdf

## COVID-19 Detection using Chest CT Scans:

### Dataset:

https://github.com/abr-98/COVID_dataset/tree/main/COVID_CT

Contains 12058 images of processed city scan images of chest of patients, the metadata contains the labels. Images are present in '.tif' format.

### Architecture

The followed Architecture is a modified approach based on the architecture proposed by the authors of: https://doi.org/10.1016/j.bspc.2021.102588. 

![Arch](https://github.com/abr-98/COVID-19-Detection-Using-Computer-vision/blob/main/Image_COVID/ARCH_CT.jpg)
 
In the publication, the defined size of the image is (512,512,1), in this work the size of the image used is reduces to (256,256,1).
The original work uses softmax and categorical cross-entropy and a 2-node output, which has been modified to 1-node in the output layer, sigmoid function, and binary-crossentropy.






