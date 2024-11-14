# **AI-Enhanced Engagement Tracker for Young Learners**  
**Infosys Springboard Internship Project, October 2024**  

### **Technologies and Libraries Used**
- **Image Processing Framework**: OpenCV  
- **Video Processing Framework**: OpenCV  
- **Annotation Tools**: OpenCV, labelImg  
- **Face Recognition Frameworks**: OpenCV, labelImg, dlib, face_recognition, imutils  
- **OpenCV Version**: 4.10.0.84  

---

## **Developed Functionalities**

### **1. Image Processing**

#### **A) Image Concatenation**
Resizes two input images to a defined pixel range and concatenates them both horizontally and vertically.
- **Functions Used**: `np.hstack()`, `np.vstack()`
- **Process**: Images are resized, concatenated side-by-side horizontally, and stacked vertically.
- **Output**: Separate windows displaying both concatenated images.

**Input**  
![download](https://github.com/user-attachments/assets/9877bd95-e226-426c-9395-bc59153199a3)

**Output**  
![image](https://github.com/user-attachments/assets/bb95e7e3-61fa-4c3d-b2ee-8705892ea3bc)

#### **B) Image Contour Detection**
Detects contours in a grayscale image.
- **Process**: Applies binary thresholding to segment the image, finds contours with `cv2.findContours()`, and overlays them in green.
- **Output**: Display of the original image with highlighted contours.

**Input**  
![OIP](https://github.com/user-attachments/assets/4a0c9a80-c161-4199-b332-6d0c3cb5ffcc)

**Output**  
![image](https://github.com/user-attachments/assets/aa14d5c1-5a83-435d-9c22-39fe5de41ef4)

#### **C) Image Crop**
Extracts a specific region from an image based on pixel coordinates.
- **Output**: Display of the cropped image in a new window.

#### **D) Image Dilation & Erosion**
Applies morphological transformations to emphasize or reduce certain image features.
- **Functions Used**: Dilation, Erosion with custom kernel matrices
- **Output**: Separate windows showing dilated and eroded versions of the image.

#### **E) Image Edge Detection**
Detects edges using the **Canny Edge Detection** algorithm.
- **Process**: `cv2.Canny()` with threshold values set to 100 and 200.
- **Output**: Window showing edges detected in the image.

#### **F) Image Histogram Equalization**
Enhances image contrast through histogram equalization.
- **Function Used**: `cv2.equalizeHist()`
- **Output**: Display of the enhanced image.

#### **G) Image Conversion to HSV**
Converts a BGR image to the HSV color space.
- **Function Used**: `cv2.cvtColor()`
- **Output**: Window showing the HSV-converted image.

#### **H) Morphological Transformation**
Applies noise reduction and fills gaps in a grayscale image.
- **Process**: `Opening` removes noise, and `Closing` fills small holes or gaps.
- **Output**: Images displayed separately, showcasing noise removal and gap filling.

#### **I) Image Resize**
Resizes an image to specified pixel dimensions.
- **Output**: Display of the resized image.

#### **J) RGB to Grayscale Conversion**
Converts a BGR image to grayscale and saves the grayscale version.
- **Function Used**: `cv2.cvtColor()`
- **Output**: Grayscale image displayed.

#### **K) Image Rotation**
Rotates the image by 90 degrees around its center.
- **Process**: Calculates the rotation matrix with a 90-degree angle using `cv2.warpAffine()`.
- **Output**: Display of the rotated image.

#### **L) Image Blur**
Applies a Gaussian blur with a 15x15 kernel to reduce noise.
- **Output**: Window showing the blurred image.

#### **M) Image Noise Removal & Closing Gaps**
Performs **Opening** and **Closing** operations to remove noise and close gaps.
- **Output**: Displayed with Matplotlib in grayscale for easy visualization.

#### **N) Template Matching**
Locates a template image within a larger image using `cv2.matchTemplate()`.
- **Process**: Highlights the matched area with a green rectangle.
- **Output**: Image with the matching region marked.

---

### **2. Video Processing**

#### **A) Multi-Video Display**
Reads and displays all images in a specified directory.
- **Process**: Iterates over folder images, showing each with dimensions.
- **Output**: Images displayed individually with a key press to move to the next.

#### **B) FPS Calculation**
Calculates and displays frames per second in a live video feed.
- **Output**: Real-time video feed with FPS calculated.

#### **C) Video Capture and Save**
Records video from the webcam and saves it to an output file.
- **Process**: Displays feed, records at a defined frame rate, and saves upon stopping.
- **Output**: Saved video in defined resolution and FPS.

#### **D) Side-by-Side Video Stacking**
Reads two video files, resizes frames, and concatenates them side-by-side.
- **Output**: Combined video displayed in real-time.

#### **E) Real-Time Video Stream**
Captures live webcam video, displaying it in a window until stopped.

---

### **3. Annotations**

#### **A) Data Segregation**
Separates images and labels into **Matched** and **Unmatched** directories based on file matching.

#### **B) Label Application**
Draws bounding boxes on images using annotations from label files, saving labeled images to output directories.

#### **C) Label Manipulation**
Updates class numbers in label files, supporting object detection and annotation tasks.

---

### **4. Face Recognition**

#### **Modules and Functionalities**
- **Face Recognition**
- **Attendance Save**
- **Test**
- **Tools**
- **Excel Save & Date Tracking**: (`excel_sc`, `excel_sc_dt`)
- **Landmark Detection**
- **Attendance Scoring**: (`atten_score`, `avg_atten_score`)

**Libraries**: OpenCV, labelImg, dlib, face_recognition, imutils
