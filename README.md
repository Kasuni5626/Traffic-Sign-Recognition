🚦 Intelligent Traffic Sign Recognition System
CNN-Based Multi-Class Image Classification


________________________________________
📌 Project Overview
This project implements a Convolutional Neural Network (CNN) to classify traffic sign images using the German Traffic Sign Recognition Benchmark (GTSRB) dataset.
The system automatically identifies traffic signs from images and demonstrates the application of deep learning in intelligent transportation systems.
This implementation serves as the baseline model (Implementation 1) for further optimization and enhancement.
________________________________________
👥 Team – SensoryX
Name	Registration Number	Index No
L.B. K. B. Sewwandi	ICT/2022/019	5626
H. T. D. Fernando	ICT/2022/020	5627
K. D. A. Nethmini	ICT/2022/026	5633
H. M. P. Theekshana	ICT/2022/070	5674
P. L. S. Fernando	ICT/2022/094	5697
Course: ICT 3212 – Introduction to Intelligent Systems
University: Rajarata University of Sri Lanka
________________________________________
📂 Dataset Information
•	Dataset: German Traffic Sign Recognition Benchmark (GTSRB)
•	Source: Kaggle
•	Classification Type: Multi-class
•	Number of Classes: 42
•	Image Type: RGB
•	Image Size: 64 × 64 pixels
Dataset Split
•	Training: 70% (6836 images)
•	Validation: 10%
•	Test: 20% (1709 images)
The test dataset was not used during training to ensure unbiased evaluation.
________________________________________
🖼️ Image Preprocessing
•	Image resizing to 64 × 64
•	Pixel normalization: [0, 255] → [0, 1]
•	Data augmentation to improve generalization
These steps ensure stable training and better performance.
________________________________________
🧠 Model Architecture
The CNN model consists of:
•	3 Convolutional layers (32, 64, 128 filters)
•	MaxPooling layers
•	Flatten layer
•	Dense layer (256 neurons, ReLU)
•	Dropout (0.5)
•	Output layer (Softmax – 42 classes)
Model Compilation
•	Optimizer: Adam
•	Loss Function: sparse_categorical_crossentropy
•	Evaluation Metric: Accuracy
________________________________________
🏋️ Training Configuration
•	Epochs: 30
•	Batch Size: 32
•	Early Stopping Patience: 5
________________________________________
📊 Results
Metric	Value
Training Accuracy	99.24%
Training Loss	0.0286
Test Accuracy	98.94%
The model demonstrates strong generalization with minimal overfitting.
________________________________________
📈 Evaluation
•	Confusion Matrix generated
•	Training vs Validation Accuracy plotted
•	Training vs Validation Loss plotted
Minor temporary overfitting observed but not sustained.
________________________________________
💾 Model Saving
•	Format: .h5
•	Save Path:
/content/drive/MyDrive/TrafficSignProject/traffic_sign_model.h5
The saved model can be reused for inference or deployment.
________________________________________
🛠️ Technologies Used
Programming Language
•	Python
Libraries
•	TensorFlow
•	Keras
•	NumPy
•	Matplotlib
Development Environment
•	Google Colab
•	Google Drive
________________________________________
🔍 Model Limitations
•	Basic CNN architecture
•	Small image size (64×64)
•	No transfer learning
•	Evaluation mainly accuracy-based
Future implementations can incorporate transfer learning and architecture improvements.
________________________________________
🚀 Conclusion
A functional CNN-based traffic sign recognition system was successfully developed.
This baseline model establishes a strong foundation for further performance optimization and deployment in intelligent transportation applications.
________________________________________
