

* Not Straight runnable out of the box. Each code chunk does a specifc task and some need to be ran independently.

* FCOS was purposed by students at The University of Adelaide in Austrialia. Their full paper and details can be found at https://paperswithcode.com/paper/fcos-fully-convolutional-one-stage-object.

* FCOS uses fully convolutional one-stage object detection to detect objects. It works by prediction a 4D vector encoding the location of the bounding boxes as shown in the image below.
  ![image](https://github.com/WillieBall/Image-Detection-Using-FCOS/assets/47549002/7f3c0d5e-8039-4f1a-86be-ffcd838555e2)

* FCOS looks to speed up the process of object detection allowing it detect objects faster than other widely used methods. Good for projects that want speed over full accuracy.
* Below is a diagram of the network architecture.
  ![image](https://github.com/WillieBall/Image-Detection-Using-FCOS/assets/47549002/a1e28b8a-2133-43de-b73d-7baf3bbb5c81)

* The Two main formulas used in this method are listed below. They are used to find the bounding boxes
* ![image](https://github.com/WillieBall/Image-Detection-Using-FCOS/assets/47549002/756e9538-f731-4d45-b33c-2f62976a797f)

* Below is a video of this code running for use in CSE470(Advanced Image Processing)
* https://drive.google.com/file/d/1nioJ5HQ7tSuXHnqUvmQuxRurYSy-bcLa/view?usp=sharing

* In their paper they claim that FCOS has a average accuracy of 44.7% with single-model and single-scale testing. From the results I got this seems to be about right
* Below are the AP(Average Precision) of images that I used in my implementation
  ![image](https://github.com/WillieBall/Image-Detection-Using-FCOS/assets/47549002/1b1cea60-deda-4c88-a204-5e64fe2efc95)
  ![image](https://github.com/WillieBall/Image-Detection-Using-FCOS/assets/47549002/7c39313f-bf8d-4290-bf98-0137c8f7f668)
  ![image](https://github.com/WillieBall/Image-Detection-Using-FCOS/assets/47549002/2cd62a4d-45db-4ab9-a54a-c728ea069908)

* In this project I initially used YOLOv2 to compare to FCOS. The AP percentage was only slighly less using FCOS than with YOLOv2, however I did notice that YOLOv2 was able to detect more images than FCOS was able to, atleast with my implementation of FOCOS.
* Below is a table of what the creators claim to be the AP percentages of other popular object detection methods compared to FCOS using different backbones.
  ![image](https://github.com/WillieBall/Image-Detection-Using-FCOS/assets/47549002/63237255-bf20-4105-92d7-55b250f514be)

* So the main advantage of FCOS is avoids computations associated with pre-defined anchor boxes. In my testing FCOS was about twice as fast as YOLOv2 was.

* This project also uses mmdetection which is an open source detection toolbox based on Pytorch which can be found at https://github.com/open-mmlab/mmdetection.




