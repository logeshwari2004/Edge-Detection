# Edge-Detection
## Aim:
To perform edge detection using Sobel, Laplacian, and Canny edge detectors.

## Software Required:
Anaconda - Python 3.7

## Algorithm:
### Step1:
import the required packages

### Step2:
Read the image and cconvert into gray image

### Step3:
remove the noise of the image using gaussian operator

### Step4:
find the sobel edge,laplacian edge,canny edge using the built in modules available in opencv

### Step5:
plot the edged image using matplotlib
 
## Program:
```
Developed by:LOGESHWARI.P
Register number:212221230055
## SOBEL EDGE DETECTOR
### sobel x:
sobelx = cv2.Sobel(new_image,cv2.CV_64F,1,0,ksize = 5)
plt.figure(figsize=(8,8))
plt.subplot(1,2,1)
plt.imshow(new_image,cmap = 'RdPu')
plt.title('RdPu')
plt.subplot(1,2,2)
plt.imshow(sobelx,cmap = 'RdPu')
plt.title("Sobel X")
plt.xticks([])
plt.yticks([])
plt.show()

### sobel y:
sobely = cv2.Sobel(new_image,cv2.CV_64F,0,1,ksize = 5)
plt.figure(figsize = (8,8))
plt.subplot(1,2,1)
plt.imshow(new_image,cmap = 'OrRd')
plt.title('OrRd')
plt.subplot(1,2,2)
plt.imshow(sobely,cmap = 'OrRd')
plt.title("Sobel Y")
plt.xticks([])
plt.yticks([])
plt.show()

### sobel xy:
sobelxy = cv2.Sobel(new_image,cv2.CV_64F,1,1,ksize=5)
plt.figure(figsize = (8,8))
plt.subplot(1,2,1)
plt.imshow(new_image,cmap = 'BuPu')
plt.title('BuPu')
plt.subplot(1,2,2)
plt.imshow(sobelxy,cmap = 'BuPu')
plt.title('Sobel XY')
plt.xticks([])
plt.yticks([])
plt.show()

## LAPLACIAN EDGE DETECTOR:
laplacian = cv2.Laplacian(new_image,cv2.CV_64F)
plt.figure(figsize = (8,8))
plt.subplot(1,2,1)
plt.imshow(new_image,cmap = 'bone')
plt.title('bone')
plt.subplot(1,2,2)
plt.imshow(laplacian,cmap = 'bone')
plt.title('Laplacian')
plt.xticks([])
plt.yticks([])
plt.show()

## CANNY EDGE DETECTOR
canny_edge = cv2.Canny(new_image,120,150)
plt.figure(figsize = (8,8))
plt.subplot(1,2,1)
plt.imshow(new_image,cmap = 'gist_gray')
plt.title('gist_gray')
plt.subplot(1,2,2)
plt.imshow(canny_edge,cmap = 'gist_gray')
plt.title('Canny Edges')
plt.xticks([])
plt.yticks([])
plt.show()

```
## Output:
### SOBEL EDGE DETECTOR
sobel x:
![DIP7A](https://user-images.githubusercontent.com/94211349/232272401-2a09e9e3-cb8a-4ee3-8a47-fad9d8c7805f.png)

sobel y:
![DIP7B1](https://user-images.githubusercontent.com/94211349/232272533-83b1f7d0-8a83-4370-9f64-ec089bc967df.png)


sobel xy:
![DIP7C](https://user-images.githubusercontent.com/94211349/232272420-6bd52b75-d080-4ba9-9452-e4fe6d133def.png)

### LAPLACIAN EDGE DETECTOR
![DIP7D](https://user-images.githubusercontent.com/94211349/232272428-66a6b654-4409-4c23-a1a5-310108d5090e.png)

### CANNY EDGE DETECTOR
![DIP7E](https://user-images.githubusercontent.com/94211349/232272437-7e9f507a-01bd-4909-929a-5bef20c90fa1.png)


## Result:
Thus the edges are detected using Sobel, Laplacian, and Canny edge detectors.
