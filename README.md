# OPENING--CLOSING
## Aim
To implement Opening and Closing using Python and OpenCV.

## Software Required
1. Anaconda - Python 3.7
2. OpenCV

## Algorithm:

### Step1: Import the necessary packages.
### Step2: Read the image.
### Step3: Create the structuring element or kernal element.
### Step4: Use Opening operation.
### Step5: Use Closing Operation.

## Program:

```
import cv2
import numpy as np
img=np.zeros((100,500),dtype='uint8')
font=cv2.FONT_HERSHEY_PLAIN
cv2.putText(img,'FAREED',(5,60),font,2,(255),5,cv2.LINE_AA)
cv2.imshow("Original Image",img)

kernal=np.ones((5,5),np.uint8)
imgO=cv2.morphologyEx(img,cv2.MORPH_OPEN,kernal)
cv2.imshow("Opening Operation",imgO)
imgC=cv2.morphologyEx(img,cv2.MORPH_CLOSE,kernal)
cv2.imshow("Closing Operation",imgC)
cv2.waitKey(0)
```
## Output:

### Display the input Image
![WhatsApp Image 2023-11-13 at 20 19 03_26f0d2ee](https://github.com/MOHAMED-FAREED-22001617/OPENING--CLOSING/assets/121412904/9615951c-7212-4866-bd51-5f573d540522)

### Display the result of Opening
![WhatsApp Image 2023-11-13 at 20 19 03_058bd51c](https://github.com/MOHAMED-FAREED-22001617/OPENING--CLOSING/assets/121412904/7e2ef35b-b469-4d2e-8445-f1313757d29a)

### Display the result of Closing
![WhatsApp Image 2023-11-13 at 20 19 03_9eb64c9e](https://github.com/MOHAMED-FAREED-22001617/OPENING--CLOSING/assets/121412904/8438e77b-7719-4b9b-8469-df1b0f088dbd)


## Result
Thus the Opening and Closing operation is used in the image using python and OpenCV.
