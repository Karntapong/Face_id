# Face Recognition System

A robust face recognition system leveraging Siamese networks with the Xception encoder, MTCNN for face detection, and clustering with DBSCAN. The system performs registration and login processes by comparing embeddings and identifying registered faces with high accuracy.

## Features
- **Face Detection**: Utilizes MTCNN to detect faces and ensures proper padding for optimal cropping.
- **Data Augmentation**: Enhances face images with transformations like rotation, brightness adjustment, flipping, and blurring for better generalization.
- **Clustering**: Employs DBSCAN to identify core embeddings and filter out noise.
- **Face Embedding**: Generates face embeddings using a Siamese network with the Xception encoder.
- **Face Registration**: Registers users by saving the mean embedding of clustered augmented images.
- **Face Login**: Verifies user identity by comparing embeddings against registered faces using Euclidean distance.
