**README for Image Enhancement Project**

---

### Project Title: Image Enhancement Techniques on Scenery Dataset

### Description
This project applies a series of image enhancement techniques on grayscale images from a specified directory. The enhancements include:
1. Histogram Equalization
2. Enhanced Contrast Stretching
3. Image Negative

Each image is processed in grayscale, and the results are displayed side by side for comparison.

### Code Summary
The code performs the following steps:
1. Loads images from a specified directory.
2. Converts each color image to grayscale.
3. Applies three enhancement techniques: 
   - **Histogram Equalization**: Enhances the image by equalizing the intensity distribution.
   - **Enhanced Contrast Stretching**: Adjusts the contrast based on specified lower and upper percentiles.
   - **Image Negative**: Generates a negative of the grayscale image.
4. Displays the original grayscale image and each enhancement side by side using Matplotlib.

### Requirements
- Python 3.x
- OpenCV
- NumPy
- Matplotlib

### Setup Instructions
1. Install the required packages:
   ```bash
   pip install opencv-python-headless numpy matplotlib
   ```
2. Place your images in a directory and update the `image_directory` variable in the code with the directory path.

### Usage
1. Update the `image_directory` variable in the code to the path of your image dataset.
2. Run the script to see the original grayscale and enhanced images side by side.

### Functions Overview
- `enhanced_contrast_stretching(image, lower_percentile, upper_percentile)`: Enhances the contrast of the image based on specified percentiles.
- `histogram_equalization(image)`: Equalizes the histogram of a grayscale image.
- `image_negative(image)`: Creates a negative of the grayscale image.

### File Structure
```plaintext
project/
│
├── main.py                  # Main script file
├── README.md                # README file
├── images/                  # Directory to store input images
```

### Example Output
For each image, the script displays:
- Original grayscale image
- Histogram equalized image
- Contrast stretched image
- Negative image

This is a visual comparison to see how each enhancement method affects the image quality.

---

### File Names
- **Script filename**: `main.py`
