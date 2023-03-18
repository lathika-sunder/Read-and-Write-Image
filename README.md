# READ AND WRITE AN IMAGE
## AIM
To write a python program using OpenCV to do the following image manipulations.
i) Read, display, and write an image.
ii) Access the rows and columns in an image.
iii) Cut and paste a small portion of the image.

## Software Required:
Anaconda - Python 3.7
## Algorithm:
### Step1:
Choose an image and save it as a filename.jpg
### Step2:
Use imread(filename, flags) to read the file.
### Step3:
Use imshow(window_name, image) to display the image.
### Step4:
Use imwrite(filename, image) to write the image.
### Step5:
End the program and close the output image windows.
## Program:
### Developed By: 
Lathika Sunder
### Register Number: 
212221230054

### i) Read and display the image
```
import cv2
A=cv2.imread("flower.jpg",1)
cv2.imshow("212221230054",A)
cv2.waitKey(0)
```

### ii)Write the image
```
import cv2
A=cv2.imread("flower.jpg",1)
cv2.imwrite("flower.jpg",A)
cv2.imshow("flower",A)
cv2.waitKey(0)
```

### iii)Shape of the Image
```
import random
import cv2
A=cv2.imread("flower.jpg",1)
for i in range(100):
    for j in range(A.shape[1]):
        A[i][j]=[random.randint(0,255),random.randint(0,255),random.randint(0,255)]
cv2.imshow("212221230054",A)
cv2.waitKey(0)
```

### iv)Access rows and columns
```
import random
import cv2
A=cv2.imread("flower.jpg",1)
for i in range(100):
    for j in range(A.shape[1]):
        A[i][j]=[random.randint(0,255),random.randint(0,255),random.randint(0,255)]
cv2.imshow("212221230054",A)
cv2.waitKey(0)
```

### v)Cut and paste portion of image
```
import cv2
A=cv2.imread("flowwer.jpg",1)
tag=A[140:240,165:180]
A[25:125,50:65]=tag
cv2.imshow("212221230054",A)
cv2.waitKey(0)
```
## Output:

## i) To Read,display the image
![l1](https://user-images.githubusercontent.com/95066409/226088426-950d347f-e8dc-496a-abf7-f979221d8607.png)

## ii) To write the image
![l2](https://user-images.githubusercontent.com/95066409/226088435-02cbe5af-cb1f-4e18-a6a6-6a0aebdc25ae.png)


## iii) Find the shape of the Image

![l3](https://user-images.githubusercontent.com/95066409/226088444-ed30e578-1215-4ca2-9830-158fa888458c.png)

## Result:
Thus the images are read, displayed, and written successfully using the python program.



