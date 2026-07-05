# Person Identification using Computer Vision

## Project Overview

This project implements a computer vision system that automatically identifies and groups images of the same individual from an unorganized dataset. The system is designed to work under different lighting conditions, facial expressions, and viewing angles.

The project uses deep learning-based face embeddings and clustering techniques to group images belonging to the same person and assigns a confidence score to each image.

---

## Features

- Automatic face detection
- Face embedding extraction using InsightFace (ArcFace)
- Face clustering using Agglomerative Clustering
- Cosine Similarity based confidence score
- CSV output containing clustered images and confidence scores
- Works with multiple individuals without prior identity labels

---

## Technologies Used

- Python 3.x
- OpenCV
- InsightFace
- ONNX Runtime
- NumPy
- Pandas
- Scikit-learn

---

## Project Structure

```
Person_Identification/
│
├── dataset/
│   ├── person_01_0.jpg
│   ├── person_01_1.jpg
│   ├── person_02_0.jpg
│   ├── person_02_1.jpg
│   ├── person_03_0.jpg
│   └── person_03_1.jpg
│
├── person_clusters.csv
├── main.py
├── README.md
└── requirements.txt
```

---

## Installation

Install the required libraries:

```bash
pip install insightface
pip install onnxruntime
pip install opencv-python
pip install numpy
pip install pandas
pip install scikit-learn
```

Or install all dependencies using:

```bash
pip install -r requirements.txt
```

---

## How to Run

1. Place all images inside the **dataset** folder.

2. Run the Python script:

```bash
python main.py
```

3. The system will:

- Detect faces
- Extract face embeddings
- Cluster images of the same person
- Calculate confidence scores
- Generate a CSV file

---

## Output

The generated CSV file contains:

| Image Name | Cluster | Confidence (%) |
|------------|---------|----------------|
| person_01_0.jpg | Person_1 | 85.36 |
| person_01_1.jpg | Person_1 | 85.36 |
| person_02_0.jpg | Person_2 | 78.80 |
| person_02_1.jpg | Person_2 | 78.80 |
| person_03_0.jpg | Person_3 | 86.34 |
| person_03_1.jpg | Person_3 | 86.34 |

---

## Methodology

1. Face Detection
2. Face Embedding Extraction
3. Feature Normalization
4. Cosine Similarity Calculation
5. Agglomerative Clustering
6. Confidence Score Generation
7. CSV Export

---

## Advantages

- No manual labeling required
- Robust to different lighting conditions
- Handles pose variations
- Handles facial expression changes
- Automatically groups images of the same individual

---

## Future Improvements

- Real-time face recognition
- RetinaFace based face detection
- Face tracking in videos
- Support for larger datasets
- Web-based interface

---

## Author

Hemant Singh

B.Tech Computer Science & Engineering

University of Engineering & Management, Jaipur# FaceCluster-AI
An AI-powered computer vision system that automatically identifies and clusters images of the same person across varying lighting conditions, poses, and facial expressions using InsightFace, cosine similarity, and Agglomerative Clustering.
