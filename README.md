# X-Ray-Image-Classification

## Abstract
We train a Convolutional Neural Network (CNN) to classify lung X-Rays into one of three categories: COVID, Normal, or Pneumonia. 

We use the tensorflow library to build a CNN that is trained on 251 grayscale images of size 255 by 255 pixels. The optimized CNN is 94% accurate on a set of 66 test images. We then compare this to another CNN built using transfer learning from the Inception.V3 Neural Net trained on ImageNet. The transfer learned model was 89% accurate on the same dataset. 

In this experiment we use tensorflow tools such as preprocessing layers, data pipeline optimization, the Keras Tuner for Hyperband tuning, and we present the results with classification reports and confusion matrices from scikitlearn. 

## Further Remarks
We also attempted to compare these two models to a much larger ResNet model with 50m trainable parameters however this model performed poorly on the testing dataset due to quickly overfitting the small dataset. 

Additionally we tried using doing transfer learning with models from tensorflow hub but as of August 2022 the tensorflow hub models do not allow for fine-tuning fractions layers of the base models. These models did not perform as well for this experiemnt as the pretrained models taken from Keras library. 

Link to CNN model in my Google Drive:
https://drive.google.com/drive/folders/10rLPUYXvjcLl9NVUvWVzC7dZHLI3P7Ce?usp=sharing

Link to Transfer Learning model in my Google Drive:
https://drive.google.com/drive/folders/1rbPhGHhtrmCWYHE2ZNvXGSgbx8ggvBZC?usp=sharing
