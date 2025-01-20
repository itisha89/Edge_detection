# README: Image Processing and Analysis

## Overview
This project involves processing an input image through multiple stages, including grayscale conversion, edge detection, segmentation, and visualization enhancements. The results are analyzed to identify the most effective techniques for edge detection and segmentation, with additional aesthetic features added to the final outputs.

---

## Workflow

### 1. **Upload and Display the Image**
- The input image is loaded and displayed in its original form.
- The image is converted to **grayscale** for further processing.

---

### 2. **Edge Detection on Grayscale Image**
Several edge detection techniques were applied to the grayscale image to identify edges:
- **Roberts**
- **Sobel**
- **Prewitt**
- **Frangi**
- **Canny** (tested with various sigma values)
- **Zero Crossing**

**Results:**
- Most techniques performed well, but **Zero Crossing** did not yield satisfactory results for the given image.

---

### 3. **Segmentation**
The grayscale image was segmented using the following techniques:
- **K-means Clustering**
- **Support Vector Machines (SVM)**
- **Convolutional Neural Networks (CNN - Deep Learning)**

**Note:** The segmented image obtained using the **CNN-based deep learning technique** was selected for further analysis due to its superior performance.

---

### 4. **Edge Detection on Segmented Image**
- The segmented image obtained from the CNN technique was processed for edge detection.
- The **Canny edge detection** method was applied with various sigma values.
- **Best Result:** Using sigma = 12.

---

### 5. **Additional Features**
- The edges detected from the CNN-segmented image (Canny with sigma = 12) were enhanced by coloring them in **red**, **green**, and **blue**.
- A custom **signature** (`ITI`) was superimposed on the **original-colored image** for branding or personalization purposes.

---

## Files
1. **Input Image:** The original image file uploaded for processing.
2. **Grayscale Image:** The converted grayscale version of the input image.
3. **Edge Detection Results:** Images showing edges identified using different techniques.
4. **Segmented Images:** Results from K-means, SVM, and CNN-based segmentation.
5. **Final Enhanced Image:** The segmented image with colored edges and the superimposed signature.

---

## Usage Instructions
1. **Input Image Upload:**
   - Ensure the input image is in a supported format (e.g., JPEG, PNG).
2. **Edge Detection:**
   - Select a method based on the desired output. Canny with sigma = 12 is recommended for the segmented image.
3. **Segmentation:**
   - Use CNN-based segmentation for optimal results.
4. **Final Enhancements:**
   - Apply colored edges and signature customization as needed.

---

## Dependencies
- **Python Libraries:** OpenCV, NumPy, Scikit-learn, TensorFlow/PyTorch (for CNN), Matplotlib
- **Image Formats:** Supported formats include `.jpg`, `.png`, and `.bmp`.

---

## Results Summary
- **Best Edge Detection Technique:** Canny edge detection (sigma = 12) on CNN-segmented images.
- **Enhancements:** Colored edges and superimposed signature add aesthetic and functional value to the processed images.

