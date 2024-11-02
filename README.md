**README for Image Enhancement Project**

**Disclaimer
All codes in this project were executed on a Kaggle notebook environment, and results may vary in different settings.**

### Project Title: Image Enhancement Techniques -1

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
- **Script filename**: `Image Enhancement Techniques -1`



----------------------********************************************************************************--------------------

### Project Title: Image Enhancement Techniques -2

### Description
This project applies various morphological operations, including dilation, erosion, opening, and closing, to a set of grayscale images. It processes each image in a specified folder, saves the output of each operation in an output folder, and displays the original and processed images.

### Code Summary
The code performs the following steps:
1. Loads images from a specified directory.
2. Applies four morphological transformations to each image:
   - **Dilation**: Expands the boundaries of the foreground.
   - **Erosion**: Shrinks the boundaries of the foreground.
   - **Opening**: Erodes an image followed by dilation, removing small objects.
   - **Closing**: Dilation followed by erosion, filling small holes.
3. Saves the processed images in an output directory with descriptive filenames.
4. Displays the original and processed images in real-time for inspection.

### Requirements
- Python 3.x
- OpenCV
- NumPy
- Matplotlib

### Setup Instructions
1. Clone or download the project:
   ```bash
   git clone <repository_url>
   ```
2. Install the required packages:
   ```bash
   pip install opencv-python-headless numpy matplotlib
   ```
3. Place your input images in the specified `image_folder` and adjust the folder paths in the script as needed.

### Usage
Run the main script to process images, save outputs, and display each image with its processed versions:
```bash
python main.py
```

### File Structure
```plaintext
project/
│
├── main.py                  # Main script file
├── README.md                # README file
├── image_folder/            # Directory to store input images
└── output_folder/           # Directory for processed images
```

### Results
After running the script, processed images will be available in the specified `output_folder` with filenames describing each operation:
- `<filename>_dilated.jpg`
- `<filename>_eroded.jpg`
- `<filename>_opened.jpg`
- `<filename>_closed.jpg`

Each image result is also displayed in the console output.

### Disclaimer
This project is intended for educational and research purposes only. The processed images and operations provided by this software should not be used as a substitute for professional image processing in any critical field, such as medical imaging or safety-critical applications. The authors make no warranties, express or implied, about the performance or suitability of this software, and they shall not be held liable for any damages arising from its use.

--- 

### File Names
- **Script filename**: `Image Enhancement Techniques-2`



