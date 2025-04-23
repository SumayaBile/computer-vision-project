## Computer Vision Project

This project implements an image stitching algorithm to create panoramas from two input images using Python and OpenCV. It demonstrates fundamental techniques in computer vision, including feature detection, keypoint matching, and image transformation.

## 🧠 Core Concepts

- **Image Stitching:** The process of combining multiple images to create a seamless panorama.
- **Feature Detection:** Detecting distinctive keypoints in an image (using algorithms like SIFT, SURF, ORB).
- **Keypoint Matching:** Matching the detected keypoints between two images.
- **Homography Estimation:** Calculating the transformation between the images to align them.

## 🗂️ Project Structure

📁 images/ ├── bryce_left_01.png └── bryce_right_01.png

📄 panorama.py # Contains the PanoramaGenerator class to generate panoramas 📄 stitch.py # Main script that loads images and performs stitching

## 🚀 How to Use

### Step 1: Prepare Your Images
Place your left and right images in the `images/` folder. Make sure they follow the naming convention:
- `*_left_*.png`
- `*_right_*.png`

### Step 2: Run the Script

```bash
python stitch.py

This will:

Load the left and right images.

Perform feature detection and keypoint matching.

Compute the homography matrix.

Generate and display the stitched panorama.

**🛠️ Requirements**
Python 3.x

OpenCV (cv2)

glob
pip install opencv-python


**🖼️ Output**
When you run the script, it will:

Display the original left and right images.

Show keypoint matches between the two images.

Display the resulting stitched panorama.

**⚙️ How It Works**
The core logic for stitching the images is contained in the PanoramaGenerator class. The class:

Takes the two input images.

Detects keypoints and matches them.

Computes the homography matrix.

Warps and aligns the images to create a panorama.

The stitch.py script is the entry point. It loads the image pairs, passes them to the PanoramaGenerator, and shows the results.










