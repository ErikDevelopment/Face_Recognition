# Face Recognition System  

## **Overview**  
This project implements a face recognition system in Python using the `face_recognition` library. It can detect faces and match them against a database of saved faces stored in a `faces` directory.  

The application utilizes a webcam to analyze video streams, identify known faces, and display their confidence levels in real-time.  

---

## **Features**  
- Real-time face detection and recognition.  
- Support for multiple known faces stored in a directory.  
- Displays names and recognition confidence directly in the video stream.  
- Optimized frame processing for improved performance.  

---

## **Requirements**  
1. **Python 3.7 or higher**  
2. Installed Python libraries:  
   ```bash  
   pip install cmake dlib==19.22 face_recognition opencv-python numpy  
   ```  

3. A folder named `faces` in the project root directory containing images of known individuals.  

4. A connected webcam or video input device.  

---

## **Installation**  

1. **Clone the repository:**  
   ```bash  
   git clone <repository-url>  
   cd <repository-directory>  
   ```  

2. **Install dependencies:**  
   ```bash  
   pip install cmake dlib==19.22 face_recognition opencv-python numpy  
   ```  

3. **Add known faces:**  
   - Save images of known individuals in the `faces` directory.  
   - The filename of each image should match the person's name (e.g., `john_doe.jpg`).  

---

## **Usage**  

1. **Run the application:**  
   ```bash  
   python main.py  
   ```  

2. **How it works:**  
   - The application starts a video stream.  
   - Known faces are identified with names and confidence levels.  
   - Press **'q'** to quit the application.  

---

## **File Structure**  
```plaintext  
📁 project-directory  
├── main.py              # Main file to start the face recognition application  
├── recognition.py       # Implementation of face recognition logic  
├── faces/               # Directory containing images of known individuals  
│   ├── person1.jpg  
│   ├── person2.jpg  
│   └── ...  
└── README.md            # This file  
```  

---

## **Common Issues**  
1. **Webcam not detected:**  
   - Ensure a webcam is connected and the correct drivers are installed.  
   - Adjust the video input index in `cv2.VideoCapture(1)` to `cv2.VideoCapture(0)` or another number.  

2. **No matches found:**  
   - Ensure the images in the `faces` directory are of high quality and the faces are clearly visible.  

---

## **License**  
This project is licensed under the MIT License.  

---

!!!**Note:** This system is intended for educational purposes only and should not be used in security-critical scenarios.!!!
