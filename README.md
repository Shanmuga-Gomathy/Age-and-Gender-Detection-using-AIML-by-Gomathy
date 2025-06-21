🧠 Real-Time Age and Gender Detection Using OpenCV DNN
This project demonstrates real-time age and gender prediction from webcam video using OpenCV's deep neural network (cv2.dnn) module and pre-trained Caffe models. It uses face detection to extract regions of interest, and applies age and gender classification to each detected face.

🔍 Features
Real-time face detection using OpenCV DNN

Age prediction across 8 age ranges:
(0-2), (4-6), (8-12), (15-20), (25-32), (38-43), (48-53), (60-100)

Gender classification: Male or Female

Display of prediction results with bounding boxes and confidence scores

Optimized with frame resizing and padding for faster inference

📁 File Structure
Copy
Edit
.
├── age_deploy.prototxt
├── age_net.caffemodel
├── gender_deploy.prototxt
├── gender_net.caffemodel
├── opencv_face_detector.pbtxt
├── opencv_face_detector_uint8.pb
└── age_gender_detection.py
🚀 Getting Started
Install Dependencies:

bash
Copy
Edit
pip install opencv-python
Run the App:

bash
Copy
Edit
python age_gender_detection.py
Requirements:

Python 3.6+

OpenCV (with DNN module)

A webcam for real-time input

📦 Models Used
Face Detection: opencv_face_detector_uint8.pb (TensorFlow model)

Age Estimation: age_net.caffemodel

Gender Classification: gender_net.caffemodel

All models must be placed in the same directory as the script.

🧪 Example Output
Terminal:

yaml
Copy
Edit
Gender : Male, conf = 0.998
Age : (25-32), conf = 0.761
On screen: Bounding box with predicted gender and age label.

