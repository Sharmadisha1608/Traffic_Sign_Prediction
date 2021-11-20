## Traffic Signs Prediction

##### Traffic sign classification is the process of automatically recognizing traffic signs along the road, including speed limit signs, yield signs, merge signs, etc. Being able to automatically recognize traffic signs enables us to build “smarter cars”. Self-driving cars need traffic sign recognition in order to properly parse and understand the roadway. Similarly, “driver alert” systems inside cars need to understand the roadway around them to help aid and protect drivers.Traffic sign recognition is just one of the problems that computer vision and deep learning can solve.
##### In this I have trained traffic sign classifier/recognizer capable of obtaining over 95% accuracy using Keras and Deep Learning.

##### Flowchart: 

![image](https://user-images.githubusercontent.com/56456928/142738081-361f462d-c81d-4a9c-acb2-80fd42b344cb.png)


##### Dataset : We have taken the dataset from German Traffic Sign Benchmark single-image classification challenge held at the International Joint Conference on Neural Networks (IJCNN) 2011 .
#####  Retrieving the images: We will retrieve the images and their labels. Then resize the images to (30,30) as all images should have same size for recognition. Then convert the images into numpy array.
##### Building the model : For building the we will use sequential model from keras library. Then we will add the layers to make convolutional neural network. In the first 2 Conv2D layers we have used 32 filters and the kernel size is (5,5). In the MaxPool2D layer we have kept pool size (2,2) which means it will select the maximum value of every 2 x 2 area of the image. By doing this dimensions of the image will reduce by factor of 2. In dropout layer we have kept dropout rate = 0.25 that means 25% of neurons are removed randomly.

##### Input Screenshot:

![image](https://user-images.githubusercontent.com/56456928/142738124-0ee6b075-ec21-4f89-b983-22614eebe4fa.png)

##### Output Screenshot:

![image](https://user-images.githubusercontent.com/56456928/142738130-9d67fa1c-5102-4818-917b-76dee45da3a4.png)
