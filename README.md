# CV_Breast-Cancer-Recognition
This project aims at constructing a binary classifier to accurately decide whether a tumor is benign or malignant.
Several networks are utilized respectively to achieve this goal and the corresponding comparison of their the performance are made.

Note that the original dataset is biased, hence I added a data augmentation step to balance the image dataset.

Below is a handdrawn schematic diagram to show the basic structure of the network.

![image](https://github.com/jerilynliu/CV_Breast-Cancer-Recognition/blob/master/Images/network_structure.png)

The original dataset contains 672 benign images and 1471 malignant images, which is clearly unbalanced and would affect the performance of the network.

<p align =“center”><img width="450" height="300" src="https://github.com/jerilynliu/CV_Breast-Cancer-Recognition/blob/master/Images/oridata.png"/></ p>

I used function data_genertor() to generate 800 benign images (by flippling, rotaion).

<p align =“center”><img width="450" height="300" src="https://github.com/jerilynliu/CV_Breast-Cancer-Recognition/blob/master/Images/augmented_data.png"/></ p>



FIve kinds of networks are utilized, namely DenseNet201, ResNet50, InceptionV3, InceptionResNet and NasNetMobile. Each network was fed the same balanced dataset. 

For comparison, DenseNet201(baseline) was fed the unbalanced dataset in order to show the importance of data augmentation.


