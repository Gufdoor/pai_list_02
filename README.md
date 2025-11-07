---

# PAI - Lista 02

## Overview

This project contains the implementation of two image processing exercises using the **scikit-image** library.
Both exercises use Google Colab for execution and visualization.

---

## Requirements

To run the code, you will need:

* Python 3.10+ (recommended through Google Colab)
* Libraries:

  * numpy
  * matplotlib
  * scikit-image
  * google.colab (for file upload)

All libraries are available by default in Google Colab.

---

## Instructions to Test

1. Open the file `pai_lista_02.py` or the corresponding Colab notebook.
2. Run all cells in order.
3. When prompted, upload **three image files** (any grayscale or RGB images).
4. The code will:

   * Apply **Otsu** and **Laplace** segmentation to each image.
   * Save the first segmented image and use it in Question 2.

---

## Question 01 – Otsu and Laplace

**Goal:** Apply two classical segmentation algorithms to three input images.

* **Otsu Thresholding:** Automatically finds the intensity value that best separates background and foreground.
  Output: Original image, histogram with threshold line, and binary segmentation.

* **Laplace (Zero-Crossing):** Detects borders by identifying abrupt intensity changes through the Laplacian operator.
  Output: Original image, Laplacian response, and detected edges.

Both algorithms are visualized side by side for comparison.

---

## Question 02 – Skeletonize

**Goal:** Represent the geometry of a segmented region using the skeletonization technique.

Steps:

1. The first image segmented by Otsu is selected.
2. The first connected region (object) from the binary mask is isolated.
3. The `skeletonize` method from `skimage.morphology` is applied to that region.
4. The original, binary, selected region, and skeleton images are displayed.

---
