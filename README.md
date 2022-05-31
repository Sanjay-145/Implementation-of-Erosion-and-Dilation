# IMPLEMENTATION OF EROSION AND DILATION
## AIM:
To implement Erosion and Dilation using Python and OpenCV.
## SOFTWARE REQUIRED:
1. Anaconda - Python 3.7
2. OpenCV
## ALGORITHM:
### Step 1:
Import the necessary packages.
### Step 2:
Create the Text using cv2.putText
### Step 3:
Create the structuring element.
### Step 4:
Erode the image.
### Step 5:
Dilate the image.

## PROGRAM:
### Developed by   : P.Sanjay
### Register Number: 212220230042

# Import the necessary packages
```
import cv2
import numpy as np
import matplotlib.pyplot as plt
```

# Create the Text using cv2.putText
```
img1=np.zeros((100,400),dtype='uint8')
font=cv2.FONT_ITALIC
cv2.putText(img1,'BOVEN',(5,70),font,2,(255),5,cv2.LINE_AA)
plt.axis('off')
plt.imshow(img1)
plt.show()
```

# Create the structuring element
```
kernel=cv2.getStructuringElement(cv2.MORPH_CROSS,(9,9))
```

# Erode the image
```
image_erode1=cv2.erode(img1,kernel)
plt.axis('off')
plt.imshow(image_erode1)
plt.show()
```

# Dilate the image
```
image_dilate1=cv2.dilate(img1,kernel)
plt.axis('off')
plt.imshow(image_dilate1)
plt.show()
```

## Output:

### Display the input Image

![S1](https://user-images.githubusercontent.com/75235426/169962465-ce43a239-6647-4475-ae48-22624e48af64.jpg)

### Display the Eroded Image

![S2](https://user-images.githubusercontent.com/75235426/169962477-7247f90c-570f-4adc-838c-6fa5f31cf064.jpg)

### Display the Dilated Image

![S3](https://user-images.githubusercontent.com/75235426/169962489-37e33c45-99fe-41cf-bceb-214713276176.jpg)

## Result
Thus the generated text image is eroded and dilated using python and OpenCV.
