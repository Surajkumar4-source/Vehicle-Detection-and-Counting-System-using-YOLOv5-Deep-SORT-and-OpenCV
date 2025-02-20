# Vehicle Detection and Counting System

## Project Overview
The **Vehicle Detection and Counting System** is a real-time computer vision application designed to detect, classify, track, and count vehicles from video feeds. This system is intended to optimize traffic monitoring and management by providing accurate data on vehicle flow. It distinguishes between different types of vehicles (e.g., cars, buses, trucks) and tracks their movement using cutting-edge machine learning models and computer vision techniques.

## Key Features
- **Real-time Vehicle Detection and Tracking:** Continuously identifies and tracks moving vehicles.
- **Vehicle Classification:** Differentiates between various vehicle types such as cars, buses, and trucks.
- **Automatic Vehicle Counting:** Counts vehicles as they pass a virtual line.
- **User-Friendly Web Interface:** Streamlit-powered dashboard for easy video upload, processing, and results visualization.
- **Data Recording:** Logs vehicle count data for future analysis and report generation.

## Tools and Technologies
- **Python:** Primary programming language.
- **OpenCV:** Image processing and video frame analysis.
- **YOLOv5:** State-of-the-art object detection model for vehicle recognition.
- **Deep SORT:** Robust object tracking algorithm for vehicle movement tracking.
- **NumPy:** Library for numerical operations and matrix manipulation.
- **Streamlit:** Framework for building an interactive web-based user interface.
- **Anaconda:** Environment and package manager to handle dependencies.

## Implementation Details
### 1. Environment Setup
- Installed essential libraries: OpenCV, NumPy, Streamlit, PyTorch, TorchVision.
- Set up YOLOv5 and Deep SORT with necessary dependencies.

### 2. Video Processing
- Captured video frames using OpenCV.
- Preprocessed frames (grayscale conversion, noise reduction) to enhance detection accuracy.

### 3. Vehicle Detection with YOLOv5
- Utilized YOLOv5 model for object detection.
- Extracted bounding boxes, class labels, and confidence scores for each detected vehicle.

### 4. Vehicle Tracking with Deep SORT
- Integrated Deep SORT to track vehicles across video frames.
- Assigned unique IDs to each vehicle to avoid multiple counts.

### 5. Vehicle Classification
- Classified detected vehicles into categories like cars, buses, and trucks based on YOLOv5 labels.

### 6. Vehicle Counting Mechanism
- Defined a virtual counting line in the video feed.
- Counted vehicles as they crossed the line, avoiding double counting using object tracking.

### 7. Web Application with Streamlit
- Developed an interactive dashboard using Streamlit.
- Features:
  - Video file upload.
  - Real-time detection visualization (video with bounding boxes).
  - Display of vehicle count and breakdown by type.
  - Option to download results as a CSV file.



## Expected Output
- Real-time video feed with bounding boxes around detected vehicles.
- Live vehicle count displayed on the dashboard.
- CSV file containing the vehicle count data available for download.

## Applications
- **Traffic Monitoring:** Analyze vehicle flow at busy intersections.
- **Toll Collection:** Automate toll processing using vehicle detection.
- **Parking Management:** Monitor parking spaces and vehicle entry/exit.
- **Road Safety:** Enhance surveillance and accident detection.

## Future Enhancements
- Support for additional vehicle types like motorcycles and bicycles.
- Improve detection accuracy using more advanced deep learning models.
- Enable multi-camera feed processing for large-scale deployments.
- Integrate with cloud platforms for remote access and real-time data visualization.


## References
- **OpenCV:** https://opencv.org/
- **YOLOv5:** https://github.com/ultralytics/yolov5
- **Deep SORT:** https://github.com/nwojke/deep_sort
- **Streamlit:** https://streamlit.io/

