![Python](https://img.shields.io/badge/Python-3.x-blue?logo=python&logoColor=white)
![OpenCV](https://img.shields.io/badge/OpenCV-Computer%20Vision-green?logo=opencv&logoColor=white)
![NumPy](https://img.shields.io/badge/NumPy-Scientific%20Computing-blueviolet?logo=numpy&logoColor=white)
![Platform](https://img.shields.io/badge/Platform-Google%20Colab-orange)
![License](https://img.shields.io/badge/License-MIT-lightgrey)

# Image Processing with OpenCV (Python)

This project demonstrates **basic image processing operations** using **OpenCV and NumPy** in Google Colab.  
It covers image loading, visualization, channel manipulation, cropping, blurring, sharpening, and adaptive thresholding.

---

## 📌 Features Implemented

- Read and display an image using OpenCV
- Inspect image properties (type, shape)
- Extract and visualize individual color channels
- Convert image to grayscale
- Remove a specific color channel
- Crop a region of interest from the image
- Apply Gaussian Blur
- Apply image sharpening using a custom kernel
- Perform adaptive thresholding

---

## 🛠️ Technologies Used

- **Python**
- **OpenCV (cv2)**
- **NumPy**
- **Google Colab**

---

## 📂 Input Image

- `teddy.png`  
  (Used as the sample image for all operations)

---

## 🔍 Image Properties

- Images are stored as **NumPy arrays**
- Color format used by OpenCV: **BGR**
- Shape format:
- (height, width, channels)


---

## 🎨 Color Channel Extraction

- Blue Channel → `image[:, :, 0]`
- Green Channel → `image[:, :, 1]`
- Red Channel → `image[:, :, 2]`

Each extracted channel is a **2-D array**.

---

## ⚫ Grayscale Conversion

The image is converted from BGR to grayscale using:

```python
cv2.cvtColor(image, cv2.COLOR_BGR2GRAY)
