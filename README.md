# **AI-Enhanced Engagement Tracker for Young Learners**
### **Infosys Springboard Internship - October 2024**

#### **Image Processing with OpenCV**

This project utilizes **OpenCV** for developing various image processing functionalities to enhance engagement tracking for young learners. The project focuses on operations like image concatenation, contour detection, cropping, morphological transformations, and more.

- **Library/Framework**: OpenCV
- **Version**: 4.10.0.84

---

## **Developed Features**

### A) **Image Concatenation**
- Resizes two input images to a specified pixel range and combines them horizontally and vertically.
- Uses `np.hstack()` for horizontal concatenation and `np.vstack()` for vertical concatenation.
- Displays concatenated results in separate windows.

**Input:**
![Input Image 1](https://github.com/user-attachments/assets/9877bd95-e226-426c-9395-bc59153199a3)
![Input Image 2](https://github.com/user-attachments/assets/4a0c9a80-c161-4199-b332-6d0c3cb5ffcc)

**Output:**
![Concatenated Image](https://github.com/user-attachments/assets/bb95e7e3-61fa-4c3d-b2ee-8705892ea3bc)

---

### B) **Image Contour Detection**
- Detects contours in a grayscale image by applying a binary threshold.
- Uses `cv2.findContours()` to identify contours and draws them in green.
- Displays the contour-highlighted image in a separate window.

**Input:**
![Grayscale Input](https://github.com/user-attachments/assets/4a0c9a80-c161-4199-b332-6d0c3cb5ffcc)

**Output:**
![Contour Output](https://github.com/user-attachments/assets/aa14d5c1-5a83-435d-9c22-39fe5de41ef4)

---

### C) **Image Crop**
- Extracts a specific region from the original image based on a defined pixel range.
- Displays the cropped image in a separate window.

**Input:**
![Input Image](https://github.com/user-attachments/assets/a44f9b5a-6251-4020-8621-cdb8a941ecc1)

**Output:**
![Cropped Output](https://github.com/user-attachments/assets/d8bfd525-0d02-44c0-a372-02d2a8ea37fa)

---

### D) **Image Dilation & Erosion**
- Uses a kernel matrix to perform morphological dilation and erosion, enhancing or reducing specific features.
- Displays both dilated and eroded images in separate windows.

**Input:**
![Input Image](https://github.com/user-attachments/assets/e426342c-d132-472f-ac3d-6d8a7d9d7f85)

**Output:**
![Dilated & Eroded Output](https://github.com/user-attachments/assets/eb05eeb4-86e5-4fd6-960d-0aba939527a0)

---

### E) **Edge Detection**
- Applies **Canny Edge Detection** with threshold values of 100 and 200.
- Displays the edge-detected image in a separate window.

**Input:**
![Grayscale Input](https://github.com/user-attachments/assets/671b4832-f723-4816-9c1b-631a87ff0993)

**Output:**
![Edge Detection Output](https://github.com/user-attachments/assets/43a4e365-4793-41bd-8282-e38404e3f56f)

---

### F) **Histogram Equalization**
- Enhances the contrast of a grayscale image using histogram equalization.
- Displays the equalized image in a separate window.

**Input:**
![Grayscale Input](https://github.com/user-attachments/assets/98640483-f13c-436a-96c7-0c4a0003d686)

**Output:**
![Equalized Output](https://github.com/user-attachments/assets/ee2eadcc-2ebf-44e2-b49d-3ce756ff56bc)

---

### G) **HSV Conversion**
- Converts a BGR image to the HSV color space.
- Displays the HSV-converted image in a separate window.

**Input:**
![BGR Input](https://github.com/user-attachments/assets/b26c4076-3591-4631-b8f4-7d85f87664db)

**Output:**
![HSV Output](https://github.com/user-attachments/assets/9e4412e2-9501-47db-881b-5020a43faed3)

---

### H) **Morphological Transformation (Opening & Closing)**
- Performs `Opening` (erosion followed by dilation) to remove noise and `Closing` (dilation followed by erosion) to fill gaps.
- Displays the processed images in separate windows.

**Input:**
![Input Image](https://github.com/user-attachments/assets/744e8b69-4baa-43ed-8329-dc838f8a0c60)

**Output:**
![Morphological Transformation Output](https://github.com/user-attachments/assets/28fc43c4-f03e-4068-b6d6-12a0ac280aeb)

---

### I) **Image Resize**
- Resizes the input image to specified dimensions.
- Displays the resized image in a separate window.

**Input:**
![Input Image](https://github.com/user-attachments/assets/0c31f8d3-5465-47b5-8f52-4c28825f8a67)

**Output:**
![Resized Output](https://github.com/user-attachments/assets/c1a2006d-19a4-47c3-b4c4-657becff578d)

---

### J) **RGB to Grayscale Conversion**
- Converts a color image to grayscale using `cv2.cvtColor()` and saves the result.
- Displays the grayscale image in a separate window.

**Input:**
![Input Image](https://github.com/user-attachments/assets/d2b162f2-c5e4-4e41-9436-8f75611e0197)

**Output:**
![Grayscale Output](https://github.com/user-attachments/assets/1673a693-b249-4499-bf88-55862193a748)

---

### K) **Image Rotation**
- Rotates the image by 90 degrees around its center using `cv2.warpAffine()`.
- Displays the rotated image in a separate window.

**Input:**
![Input Image](https://github.com/user-attachments/assets/a16a3e78-45a2-47db-ad11-3c8756eb0b37)

**Output:**
![Rotated Output](https://github.com/user-attachments/assets/bd727570-7d95-4a42-ba44-1c78ada5a74c)

---

### L) **Image Blur**
- Applies a Gaussian blur with a 15x15 kernel to reduce noise and smooth the image.
- Displays the blurred image in a separate window.

**Input:**
![Input Image](https://github.com/user-attachments/assets/e3e2cfad-ab4e-4696-87bc-f7b176b06d18)

**Output:**
![Blurred Output](https://github.com/user-attachments/assets/dfe50e24-cbe3-491d-be99-e7b7b433c681)

---

Each feature has been designed to support engagement tracking for educational applications by enhancing or processing images effectively.
