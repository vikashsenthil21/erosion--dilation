## Implementation-of-Erosion-and-Dilation
### Aim
To implement Erosion and Dilation using Python and OpenCV.
### Software Required
1. Anaconda - Python 3.7
2. OpenCV
### Algorithm:
#### Step1:<br>
Import the necessary pacakages

#### Step2:<br>
Create the text using cv2.putText

#### Step3:<br>
Create the structuring element

#### Step4:<br>
Erode the image


#### Step5: <br>
Dilate the Image

 
### Program:
```
Name : Vikash s
Register no : 212222240115
```

##### Import the necessary packages
``` Python
import numpy as np
import cv2
import matplotlib.pyplot as plt
```
##### Read and show the Original image
``` Python
image = cv2.imread("vikash.png")
kernel = cv2.getStructuringElement(cv2.MORPH_RECT, (5, 5))
image_rgb = cv2.cvtColor(image, cv2.COLOR_BGR2RGB)
plt.imshow(image_rgb)
plt.title("Original Image")
plt.axis("off")
```

##### Erode the image
``` Python
eroded_image = cv2.erode(image, kernel, iterations=1)
eroded_image_rgb = cv2.cvtColor(eroded_image, cv2.COLOR_BGR2RGB)
plt.imshow(eroded_image_rgb)
plt.title("Eroded Image")
plt.axis("off")

```
##### Dilate the image
``` Python
dilated_image = cv2.dilate(image, kernel, iterations=1)
dilated_image_rgb = cv2.cvtColor(dilated_image, cv2.COLOR_BGR2RGB)
plt.imshow(dilated_image_rgb)
plt.title("Dilated Image")
plt.axis("off")



```
### Output:

#### Display the Original Image

![image](https://github.com/user-attachments/assets/69f0f87e-ee85-4f88-a0a6-7164fbf1f898)


#### Display the Eroded Image

![image](https://github.com/user-attachments/assets/f2b082b5-54e3-467b-9a5d-3d5754b14aa3)



#### Display the Dilated Image
![image](https://github.com/user-attachments/assets/f237cd11-8c07-4b99-b547-c90ff2b17216)




## Result
Thus the generated text image is eroded and dilated using python and OpenCV.
