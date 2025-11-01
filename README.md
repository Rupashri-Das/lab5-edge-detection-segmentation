# Lab 5 — Edge Detection and Segmentation (MATLAB)

This repository contains the implementation and results for Lab 5 of the Image Processing course. The purpose of this lab was to apply different edge detection operators, perform automatic thresholding, and visualize segmented regions based on binary masks.

---

## 1. Edge Detection Operators

Three edge detectors were tested:

- Sobel and Prewitt (first-order gradient filters)
- Canny (multi-stage detector with non-maximum suppression and hysteresis)
- Laplacian of Gaussian (zero-crossing method)

These operators were compared visually to observe edge sharpness, noise sensitivity, and continuity.

---

## 2. Thresholding and Segmentation

Otsu’s automatic thresholding method was used to convert the grayscale image into a binary mask.  
The resulting regions were labeled and visualized using color mapping to show the separated objects.

---

## 3. Observations

- Canny produces the thinnest and most continuous edges because it applies both Gaussian smoothing and non-maximum suppression.
- Sobel and Prewitt are simple gradient detectors but are more sensitive to noise and produce thicker edges.
- The Laplacian of Gaussian detects zero-crossings and highlights fine structures but may introduce extra noise edges.
- Otsu’s method selects a threshold by maximizing between-class variance, making it fully automatic and histogram-based.
- Region labeling helps convert edge maps and masks into meaningful segmented areas.

---

## 4. How to Run

1. Open MATLAB (Online or Desktop).
2. Run `lab5_edge_detection_segmentation.m`.
3. Save each figure manually after running the script.
4. Upload them to GitHub along with this README.

---

## 5. Environment

- MATLAB Online (R2024x or similar)
- Uses built-in `peppers.png`

---

## 6. Author

Name: Rupashri Das
Date: 1.11.2025
