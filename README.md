# Face Detection System 👤

A computer vision project that detects human faces in images and videos using **Python, OpenCV, and the pretrained YuNet face detection model**. The project includes an interactive web interface built with Gradio, allowing users to upload images or videos and visualize detected faces with bounding boxes.

## 🚀 Features

* **Image Face Detection:** Detects faces in uploaded images.
* **Video Face Detection:** Processes videos frame by frame to detect faces.
* **Face Localization:** Draws bounding boxes around detected faces.
* **Confidence Scores:** Displays detection confidence for image results.
* **Detection Statistics:** Reports the number of detected faces and video processing statistics.
* **Interactive Web Interface:** Provides an easy-to-use interface built with Gradio.

## 🛠️ Technologies Used

* **Python** — Core programming language
* **OpenCV** — Image and video processing
* **YuNet** — Pretrained face detection model
* **Gradio** — Interactive web interface
* **Matplotlib** — Image visualization
* **Google Colab** — Development and testing environment

## ⚙️ How It Works

The system uses the pretrained YuNet face detection model to identify faces in images and video frames.

1. **Input:** The user provides an image or video.
2. **Preprocessing:** OpenCV loads the input and prepares it for detection.
3. **Face Detection:** YuNet analyzes the image or individual video frames.
4. **Face Localization:** Bounding boxes are drawn around detected faces.
5. **Results:** The application displays the processed image or video and relevant detection statistics.

## 📊 Initial Testing Results

The system was tested using a sample video with the following results:

| Metric                                     |    Result |
| ------------------------------------------ | --------: |
| Video Resolution                           | 768 × 576 |
| Frame Rate                                 |    10 FPS |
| Total Frames Processed                     |       795 |
| Frames Containing Detected Faces           |       439 |
| Total Face Detections Across Frames        |       636 |
| Percentage of Frames Containing Detections |    55.22% |

**Note:** These results represent an initial demonstration, not a formal measurement of model accuracy. Face detections across multiple frames may include the same person repeatedly. Performance can vary depending on image quality, lighting, face size, and viewing angle.

## 💻 Installation

Install the required Python packages:

```bash
pip install opencv-python-headless matplotlib numpy gradio
```

Download the pretrained YuNet model from the [OpenCV Zoo repository](https://github.com/opencv/opencv_zoo/tree/main/models/face_detection_yunet).

Place the model in the following location:

```text
models/
└── face_detection_yunet_2023mar.onnx
```

## ▶️ Running the Project

The project was developed and tested in Google Colab.

1. Open the notebook `Face_Detection_ML_Project.ipynb` in Google Colab.
2. Install the required dependencies.
3. Download or provide the pretrained YuNet model.
4. Run the notebook cells in order.
5. Launch the Gradio interface.
6. Open the generated Gradio link to access the application.
7. Upload an image or video and run face detection.

**Important:** The Gradio link is temporary and generally remains available only while the Colab session is running.

## 📁 Project Structure

```text
Face-Detection-System/
│
├── Face_Detection_ML_Project.ipynb
├── models/
│   └── face_detection_yunet_2023mar.onnx
├── sample_face.jpg
├── sample_video.avi
├── face_detection_output.mp4
└── README.md
```

*The actual files in your repository may differ. Include the model, sample media, and output video only if you intend to distribute them.*

## 🎯 Applications

* Image and video analysis
* Computer vision demonstrations
* Face localization in multimedia
* Learning and experimentation with pretrained machine learning models
* Educational projects involving image processing

## ⚠️ Limitations

* The project uses a pretrained model rather than training a face detector from scratch.
* Detection performance depends on image quality, lighting, face size, and orientation.
* Small, blurred, partially hidden, or distant faces may be missed.
* Detection counts do not represent unique individuals.
* The project detects faces; it does not identify people or recognize their identities.

## 🔮 Future Improvements

* Evaluate the detector on a labelled face detection dataset.
* Measure precision, recall, and other suitable evaluation metrics.
* Add webcam-based face detection.
* Improve the interface and visualization of detection results.
* Explore alternative detection models and compare their performance.

## 📚 Acknowledgements

This project uses the pretrained YuNet face detection model from the [OpenCV Zoo](https://github.com/opencv/opencv_zoo) project and OpenCV's computer vision tools.

## 📄 License

This repository is intended for educational and learning purposes. Check the applicable licenses for the model, dependencies, and any sample media before redistributing them.

---

**Developed as a computer vision and machine learning project using Python and OpenCV.**
