# Big-Transfer-Learning
Used  the Big Transfer Learning methods described by Google Research team in conjunction with PyTorch to replicate the behavior of an upstream dataset using the ResNet50-x3 architecture. 
Used 1-10 examples per class. 
Note that this will definitely result in overfitting. For our purposes, it is okay as we are trying to replicate the behavior shown by the Google Research Team.

Link to Paper: https://arxiv.org/pdf/1912.11370.pdf


<b>What is Transfer Learning?</b>

In Machine Learning, we train every model individually, but in Transfer Learning, we
apply the knowledge acquired from the training of one dataset to another dataset / task / model.
Transfer Learning focuses on fine tuning rather than pre-training. The pre-training is done using
a very large dataset probably containing 300 million images and this pre-trained model is used
for processing small datasets.


Similar to how humans learn, we learn a certain piece of information and apply it to
another setting (i.e. calculus for artificial intelligence). The training of the network is usually
done over a large generic dataset that contains a huge amount of data. According to the paper in
scope, the datasets mentioned are BiT-L which is trained on the JFT 300 M dataset which
contains 300 million noisily labelled images, BiT-M which is trained on the ImageNet 21K
dataset containing 14 million images and the BiT-S which is trained on the ImageNet dataset
containing 1.3 million dataset.


There are two components of Transfer Learning: Pre-training and Fine-tuning.
Pre-training is where a CNN is created by allowing it to process a huge dataset. Now the purpose
of this pre-training lies in creating a network whose knowledge can be used on subsequent tasks
by a process called fine-tuning. This consists of fine-tuning the weights to fit the requirements of
the target task.


<b>Where can this be applied?</b>


Transfer learning can be used in almost any scenario where there is a need for prediction
and analysis based on prior knowledge on that particular field / task. Suppose you are training a
model that detetcts disease in lungs and the dataset containing the images of the diseased areas in
lungs is not very large. This would require a CNN that has already been pre-trained on a large
dataset of similar images. A possible solution through the means of Transfer Learning would be
first training a large dataset using a Convolutional Neural Network (CNN) and then using the
small dataset to fine tune the model.
