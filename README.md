# Computer Vision Lab 3 – Edge Detection

## Description
This program demonstrates three common edge detection techniques in Computer Vision:
- Prewitt Edge Detection
- Sobel Edge Detection
- Canny Edge Detection

The input image is converted to grayscale and processed using the three methods. The results are displayed together for comparison.

## Requirements
Install the following Python libraries:

```bash
pip install opencv-python numpy matplotlib
```

## Input Image
The program expects an image named:

`batman.jpg`

In the original Colab code, the image is loaded from:

`/content/batman.jpg`

Make sure the image is uploaded to the correct location before running the program.

## How to Run
1. Open the Python file in Google Colab or a Python environment.
2. Install the required libraries if necessary.
3. Upload/place `batman.jpg` in the expected path.
4. Run the program.
5. The output displays:
   - Original grayscale image
   - Sobel edge detection
   - Prewitt edge detection
   - Canny edge detection

## Working
### 1. Grayscale Conversion
The input image is converted from BGR format to grayscale using OpenCV.

### 2. Prewitt Edge Detection
Two 3×3 kernels are used to detect horizontal and vertical intensity changes. The two results are combined to obtain the final Prewitt edge image.

### 3. Sobel Edge Detection
Sobel filters are applied in the X and Y directions using OpenCV. Their absolute responses are combined to produce the Sobel edge image.

### 4. Canny Edge Detection
Canny edge detection is applied with threshold values of 100 and 200.

### 5. Comparison
A 2×2 plot displays the original grayscale image and the three edge-detection results.

## Libraries Used
- `cv2` – image processing and edge detection
- `numpy` – numerical operations and filter kernels
- `matplotlib.pyplot` – displaying the results

## Expected Output
The program produces a comparison figure containing four images:
1. Original grayscale image
2. Sobel edge detection
3. Prewitt edge detection
4. Canny edge detection

## Source
The Python file is a Colab-generated Computer Vision Lab 3 program.
