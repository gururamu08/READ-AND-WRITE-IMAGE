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
### Developed By: GURUMOORTHI R
### Register Number: 212222230042
i) #To Read,display the image
```
  import cv2
img=cv2.imread("dipt.jpg",1)
cv2.imshow('GURUMOORTHI R 212222230042',img)
cv2.waitKey(0)

```
ii) #To write the image
```
import cv2
img = cv2.imread('dipt.jpg', 1)
new_img = cv2.imwrite('dipt_copy.jpg', img)
cv2.imshow('GURUMOORTHI R 212222230042', img)
cv2.waitKey(0)


```
iii) #Find the shape of the Image
```python3

import cv2
img = cv2.imread('dipt.jpg', 1)
print(img.shape)

```
iv) #To access rows and columns

```python3
import cv2
import random
img = cv2.imread('dipt.jpg', 1)
for i in range(100):
    for j in range(img.shape[1]):
        img[i][j] = [random.randint(0, 255), random.randint(0, 255), random.randint(0, 255)]
cv2.imshow('part image', img)
cv2.waitKey(0)
cv2.destroyAllWindows()


```
v) #To cut and paste portion of image
```python3
import cv2
img = cv2.imread('dipt.jpg', 1)
tag = img[300:400, 300:400]
img[50:150, 50:150] = tag
cv2.imshow('GURUMOORTHI R 212222230042', img)
cv2.waitKey(0)
cv2.destroyAllWindows()


```

## Output:

### i) Read and display the image

![read and display](https://github.com/gururamu08/READ-AND-WRITE-IMAGE/assets/118707009/f43c63d0-53eb-4045-b568-9e9cc7651604)


### ii)Write the image

![write image](https://github.com/gururamu08/READ-AND-WRITE-IMAGE/assets/118707009/0bca4a51-38df-4aad-ab87-c367adafe3b7)


### iii)Shape of the Image

![shape](https://github.com/gururamu08/READ-AND-WRITE-IMAGE/assets/118707009/59e88b9e-3ef4-41c6-ba28-f61ec951a958)


### iv)Access rows and columns

![access rows and columns](https://github.com/gururamu08/READ-AND-WRITE-IMAGE/assets/118707009/ccba8211-1673-40f9-a0d6-85a2126b9931)


### v)Cut and paste portion of image

![cut and paste](https://github.com/gururamu08/READ-AND-WRITE-IMAGE/assets/118707009/5bb20689-f8ac-4102-b994-d1eb51dd85a0)


## Result:
Thus the images are read, displayed, and written successfully using the python program.
