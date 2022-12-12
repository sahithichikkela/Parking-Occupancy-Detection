# Parking Space Detection using OpenCV

This project explores the use of OpenCV, a popular image processing library, to detect parking space availability from an image or video of a parking lot.

## Project Overview
The main goal was to detect whether parking spots were occupied or available by analyzing video footage or images of parking lots. While the complete automation of the process proved challenging, the project successfully detects available parking spots with some user input.

## How It Works
1. The user provides a video or an image of a parking lot.
2. The user marks the corners of each parking spot to track.
3. The program overlays boxes on each parking spot (green for available, red for occupied).
4. As cars move in or out, the boxes change colors:
   - **Green**: Parking space is available.
   - **Red**: Parking space is occupied.

The system can be used for various purposes, such as:
- Real-time parking spot availability detection.
- Analyzing parking lot usage.
- Assisting parking lot management with available space tracking.

## Running the Program
To run the program, use the following command:
```
python main.py --image images/parking_lot_1.png --data data/coordinates_1.yml --video videos/parking_lot_1.mp4 --start-frame 400
```

## Key Features
- **Line Detection**: Uses OpenCV’s Hough Transform to detect parking spot boundaries.
- **Rectangle Drawing**: Allows users to manually mark parking spots by clicking on the image.
- **Color-coded Spots**: The program tracks and displays the availability of parking spots with colored boxes.

## Process Summary
- **Initial Setup**: Load an image or video of a parking lot.
- **User Input**: Manually mark each parking spot by selecting its corners.
- **Detection**: As cars move in and out of spots, the system updates the status of the spots.
  
## Future Improvements
- Automate the detection of parking spaces without user input.
- Improve motion detection accuracy.
- Make the system more adaptable to different parking lot layouts.

This project was a fun introduction to computer vision, using OpenCV to tackle a real-world problem. Feedback and suggestions for improvement are always welcome!