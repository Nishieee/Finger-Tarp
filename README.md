# Finger Tarp

## Introduction

Finger Tarp is a hands-free digital drawing canvas that allows users to draw on a screen by waving a finger fitted with a colored cap. Utilizing the power of computer vision via OpenCV, this project aims to provide an innovative, cost-effective solution for digital art and interactive education.

### Objectives

- Provide an alternative to traditional drawing tablets and styluses, reducing the need for expensive hardware in educational and artistic settings.
- Harness Python and OpenCV to create an intuitive interface for drawing using simple hand gestures.

## Technology Stack

- **Programming Language:** Python
- **Libraries:** OpenCV, NumPy

## Usage
- **Setup**: Attach a brightly colored cap to your fingertip. Ensure the color is consistent and distinct from your background.
- **Initialization**: Start the application and position your finger in front of your webcam.
- **Interaction**: Move your finger to draw. The application tracks your finger's position and movement, rendering these as brush strokes on your digital canvas.

## System Architecture

The application processes input in several stages:

- **Color Detection**: Identifies the color of the cap using the HSV color space.
- **Finger Tip Tracking**: Utilizes contour detection to track the movement of the colored cap.
- **Drawing**: Converts the tracked movements into brush strokes on the canvas.

## How It Works
The procedure is explained in four main steps:
1. **Color Tracking**: Detect the specific color on the finger.
2. **Detection of the Colored Point at the Finger Tip**: Locate the colored point using OpenCV's `cv.inRange()` function.
3. **Tracking the Tip**: Continuously follow the movement of the colored point.
4. **Drawing the Points**: Plot the points on the screen based on the movement tracked.

## Detailed Steps
- **Color Detector Screen**: Set the saturation value to match the color of the bead.
- **Mask Screen**: Track the bead and trace its path, providing coordinates for drawing.
- **Color Change & Tracking**: Change drawing colors based on the detected bead's coordinates.
- **Deques for Storage**: Store coordinates in deques for efficient updating and drawing in real-time.

## Conclusion and Future Scope
The Finger Tarp allows drawing as if in the air, and can be enhanced for more precise hand gesture tracking. Future developments could include more colors, brushes, textures, and saving options, potentially replacing traditional whiteboards in classrooms.

## Block Diagram
![Block Diagram - Flow](https://github.com/Nishieee/Finger-Tarp/blob/main/Images/Block%20Diagram.png)


## Future Scope
- **Gesture Recognition Enhancement**: Improve the accuracy and responsiveness of gesture tracking.
- **Brush Customization**: Introduce more options for brush size, color, and texture.
- **Save and Export Options**: Allow users to save and export their drawings in various formats.





## Installation

To set up the Finger Tarp on your local machine, follow these instructions:

```bash
# Install Python libraries
pip install opencv-python numpy

# Clone the project repository
git clone https://github.com/your-repository/finger-tarp.git

# Navigate to the project directory
cd finger-tarp

# Run the application
python fingertarp.py




 
