# Object-classification-and-detection-model-using-YOLOv3

# Objective 
# 1. Data preprocessing 
The data preprocessing phase mainly includes the methodology based on the intensity transformation technique specifically into the spatial domain to enhance the image quality before feeding into the model.

## Adjusting the Brightness and Contrast of the image
The parameters α>0 and β are often called the gain and bias parameters; sometimes these parameters are said to control contrast and brightness respectively.
		g(i,j)=α⋅f(i,j)+β 
    f(x): source image pixels and g(x) :output image pixels

### original image 

![alt text](https://github.com/gouravbarkle/Object-classification-and-detection-model-using-YOLOv3/blob/main/Image%20metadata/original.png)

### Image after tuning Brightness and Contrast

![alt text](https://github.com/gouravbarkle/Object-classification-and-detection-model-using-YOLOv3/blob/main/Image%20metadata/original%20after%20enhancement.png)


## Histogram Equalization
An image histogram gives a graphical representation of the distribution of pixel intensities in a digital image.
The x-axis indicates the range of values the variable can take. This range can be divided into a series of intervals called bins. 
The y-axis shows the count of how many values fall within that interval.

### histogram representation of original image 

![alt text](https://github.com/gouravbarkle/Object-classification-and-detection-model-using-YOLOv3/blob/main/Image%20metadata/Histo%20original.png)

### histogram representation after Equalization

![alt text](https://github.com/gouravbarkle/Object-classification-and-detection-model-using-YOLOv3/blob/main/Image%20metadata/histo%20after.png)

### Output after Histogram Equalization

![alt text](https://github.com/gouravbarkle/Object-classification-and-detection-model-using-YOLOv3/blob/main/Image%20metadata/image%20histo.jpg)


# 2. Object classification and detection using YOLO

* What is Yolo?
	* YOLO (You Only Look Once) object detection algorithm, which is one of the most effective object detection algorithms.
	* It takes the entire image in a single instance and predicts the bounding box coordinates and class probabilities for these boxes. 
	* YOLO takes input and make predictions on it in single pass only, it uses CNN in the background for task completion.  

* YOLO Architecture
	* 53 Conv layers called Darknet-53 stacked with 53 more layers producing 106 layers in total.
	* No pooling layer used here instead of pooling it uses convolution layer with a filter 1X1 to down sample the input, as a result it enables & helps to 	improve ability to detect small object.
	* YOLO V3, detects object at 3 different scales and at the layer 82,94 and 106.
	* It uses three different stride values as 32,16 and 8 for detecting different types of features from the input.  
