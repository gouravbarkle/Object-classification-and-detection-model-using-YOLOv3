# Object-classification-and-detection-model-using-YOLOv3

# Objective 
# 1. Data preprocessing 
The data preprocessing phase mainly includes the methodology based on the intensity transformation technique specifically into the spatial domain to enhance the image quality before feeding into the model.

## Adjusting the Brightness and Contrast of the image
The parameters α>0 and β are often called the gain and bias parameters; sometimes these parameters are said to control contrast and brightness respectively.
		g(i,j)=α⋅f(i,j)+β 
    f(x): source image pixels and g(x) :output image pixels


![alt text](https://github.com/gouravbarkle/Object-classification-and-detection-model-using-YOLOv3/blob/main/Image%20metadata/original.png)

### original image 

  
![alt text](https://github.com/gouravbarkle/Object-classification-and-detection-model-using-YOLOv3/blob/main/Image%20metadata/original%20after%20enhancement.png)

### Image after tuning Brightness and Contrast

## Histogram Equalization
An image histogram gives a graphical representation of the distribution of pixel intensities in a digital image.
The x-axis indicates the range of values the variable can take. This range can be divided into a series of intervals called bins. 
The y-axis shows the count of how many values fall within that interval.



# 2. ff
