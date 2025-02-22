# RF Source_detection using 1D CNN

This project uses a CNN to perform Radio Signal source detection. A 20 element array is used to estimate the number of signals impinging it.    

Estimation of the number of sources is an important step in various array processing technologies. It is a prerequisite in most DoA algorithms. This model was succesfull in recognisng upto 6 sources at 20dB of SNR. Output of the code includes plots of the training and validation error, stats(precision,sensitivity, and specificity), a confusion matrix, and the ROC plot of the test data.

Contact me at jayakrishnan@unm.edu for the data. Files are too large to be uploaded here. 
#Updated results published at - https://ieeexplore.ieee.org/document/10137757


# Architecture 

![cnn](https://user-images.githubusercontent.com/20204692/132585407-62829f0a-67ff-4f49-8a07-6cc5ea4d5458.png)

The upper triangle of the received auto-correlation matrix is flattened into a one dimensional vector and fed as the input. The output is a one hot encoded vector which denotes the number of sources present. Experiments are performed with the number of signals varying from 0-5.   

# Results 

![conf_20db](https://user-images.githubusercontent.com/20204692/132585583-ef567dd6-ec27-4d19-8d3a-707343d8e87a.png)



# References

[Code template](https://github.com/moemen95/Pytorch-Project-Template)

[Image generation for CNN model](https://github.com/ashishpatel26/Tools-to-Design-or-Visualize-Architecture-of-Neural-Network)
