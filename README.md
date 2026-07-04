# Smart SWIPE: Active Learning-based Intelligent Photo Organization

## Overview

**Smart SWIPE** is an intelligent photo organization system that leverages **Active Learning** and **Deep Learning** to automatically classify and organize large personal photo collections. Instead of requiring users to manually label thousands of images, the system learns user preferences from a small number of swipe interactions and predicts labels for the remaining images.

Developed as part of the **Summer Project** under the **Association of Computing Activities (ACA), IIT Kanpur**, Smart SWIPE aims to reduce manual effort while maintaining high classification accuracy and scalability.

---

## Motivation

Modern smartphones often contain thousands of photos, making manual organization time-consuming and inefficient. Existing gallery applications rely heavily on manual album creation and sorting.

Smart SWIPE addresses this challenge by learning from user interactions through **Active Learning**, enabling automatic organization of **5,000+ photos** after approximately **300 swipe-based labels**.

---

## Features

- Active Learning-based image classification
- Learns user preferences from minimal swipe interactions
- Automatically organizes **5,000+ images**
- Reduces manual labeling effort
- Deep learning-based feature extraction
- Continuous model improvement through user feedback
- Scalable and efficient photo management

---

## Project Pipeline

```
Photo Gallery
      │
      ▼
Image Preprocessing
      │
      ▼
Feature Extraction
      │
      ▼
Active Learning
      │
      ▼
User Swipe Feedback
      │
      ▼
Model Training
      │
      ▼
Automatic Image Classification
      │
      ▼
Organized Photo Gallery
```

---

## Methodology

### 1. Image Collection
- Import images from the user's photo gallery.
- Filter corrupted and duplicate images.

### 2. Image Preprocessing
- Resize images
- Normalize pixel values
- Perform data augmentation
- Improve image quality

### 3. Feature Extraction
Deep visual features are extracted using a pretrained Convolutional Neural Network (CNN) to generate semantic image embeddings.

### 4. Active Learning
Instead of labeling every image, the model selects the most informative samples for user feedback.

Workflow:
1. Randomly sample images.
2. User swipes to provide labels.
3. Train the classifier.
4. Select uncertain samples.
5. Repeat until convergence.

### 5. Image Classification
The trained model predicts labels for the remaining unlabeled images with confidence scores.

### 6. Continuous Learning
Every new user interaction updates the model, allowing it to adapt to changing preferences over time.

---

## Technologies Used

- Python
- PyTorch
- OpenCV
- NumPy
- TorchVision
- Scikit-learn
- Matplotlib
- Jupyter Notebook

---

## Repository Structure

```
Smart-SWIPE/
│
├── final_code.ipynb           # Complete project implementation
├── Smart_SWIPE_Project_Report.pdf
├── README.md
├── images/                    # Sample outputs (optional)
└── requirements.txt
```

---

## Evaluation Metrics

The system is evaluated using:

- Accuracy
- Precision
- Recall
- F1-score
- Classification Confidence
- Number of User Swipes
- Label Reduction Percentage
- Inference Time

---

## Expected Results

- Learn user preferences from approximately **300 swipe interactions**.
- Automatically classify and organize **5,000+ photos**.
- Reduce manual labeling effort significantly.
- Continuously improve performance through Active Learning.
- Provide a scalable and intelligent photo management solution.

---

## Applications

- Smartphone photo organization
- Cloud photo management
- Automated album creation
- Personal digital assistants
- Image retrieval systems
- Multimedia content management

---

## Future Enhancements

- Face recognition and clustering
- Event-based album generation
- Duplicate image detection
- Natural language photo search
- Vision-Language Model integration
- Cross-device synchronization
- Personalized photo recommendations

---

## How to Run

Clone the repository:

```bash
git clone https://github.com/your-username/Smart-SWIPE.git
```

Navigate to the project directory:

```bash
cd Smart-SWIPE
```

Install dependencies:

```bash
pip install -r requirements.txt
```

Launch the notebook:

```bash
jupyter notebook final_code.ipynb
```

Run all notebook cells to train the model and reproduce the results.

---

## Project Status

**🚧 Ongoing**

Current Progress:
- ✅ Data preprocessing pipeline
- ✅ Active Learning framework
- ✅ Image feature extraction
- 🔄 Model optimization
- 🔄 Performance evaluation

---

## Author

**Siddharth Kumar**  
B.Tech, Materials Science and Engineering  
Indian Institute of Technology Kanpur

---

## Acknowledgements

This project is being carried out as a **Summer Project** under the **Association of Computing Activities (ACA), IIT Kanpur**.

---

## License

This project is intended for educational and research purposes only.
