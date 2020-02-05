# CV_Breast-Cancer-Recognition
This project aims at constructing a binary classifier to accurately decide whether a tumor is benign or malignant.
Several networks are utilized respectively to achieve this goal and the corresponding comparison of their the performance are made.

Note that the original dataset is biased (600:1400), hence I added a data augmentation step to balance the image dataset.
(generated 800 benign images using data_generator function to get a 1600:1600 unbiased dataset)

Below is a handdrawn schematic diagram to show the basic structure of the network.

![image](https://github.com/jerilynliu/CV_Breast-Cancer-Recognition/blob/master/Images/network_structure.png)

I tried 5 kinds of network, namely DenseNet201, ResNet50, InceptionV3, InceptionResNet and NasNetMobile. Each network was fed the same balanced dataset. 

For comparison, DenseNet201(baseline) was fed the unbalanced dataset in order to show the importance of data augmentation.


