# MST Medical Image Segmentation

## Overview
This project applies Minimal Spanning Trees (MSTs) and a modified Kruskal's algorithm to segment and denoise medical images. It transforms grayscale images (like MRIs or CT scans) into grid graphs, merging similar pixels to identify anatomical structures while smoothing out noise. 

## Requirements
* Python 3.x
* `numpy`
* `matplotlib`
* `scikit-image`
* `scipy`

## How to Run
1. Upload your medical images (e.g., from the Brain Tumor MRI dataset) to your working directory or Google Colab session.
2. Open the main Python script.
3. Update the `image_paths` list at the bottom of the script with your specific file names:
   ```python
   image_paths = [
       '/content/Te-no_1.jpg', 
       '/content/Te-gl_1.jpg',
       '/content/Te-aug-me_1.jpg'
   ]
4. Run the script. The output will automatically display the computation time, Number of Segments, MSE, and PSNR, along with 2x2 visual grids for each image.

## Configuration

To adjust the sensitivity of the segmentation, modify the scale parameter `k` in the main execution block. A higher `k` (e.g., 500) creates larger segments, while a lower `k` creates finer, smaller segments.

## Author

Amrutha Ajish Achuthan
