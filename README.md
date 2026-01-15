# Deepfake Detection Model w/ CNNs
## ✨ Overview
![Deepfake of Arnold Schwartznagger](https://external-content.duckduckgo.com/iu/?u=https%3A%2F%2Fstatic1.srcdn.com%2Fwordpress%2Fwp-content%2Fuploads%2F2020%2F02%2FTerminator-Deepfake.jpg&f=1&nofb=1&ipt=b31a8af41122b3f29dce2ccedfc7695c278d938cf7b67f93f0ede4f938719273&ipo=images)

This project explores the use of convolutional neural networks (CNNs) to detect deepfake images by identifying visual artifacts introduced during face manipulation. The model is inspired by the <a href="https://arxiv.org/abs/1809.00888">Mesonet architecture</a> and focuses on capturing subtle spatial inconsistencies rather than high-level facial features.


## 🔍 Approach

- Extract and preprocess facial image data from real and manipulated sources

- Train a CNN inspired by MesoNet to capture spatial inconsistencies

- Perform binary classification (real vs. deepfake) at the image level

- Output prediction confidence scores to surface model uncertainty

The model intentionally operates on individual frames and does not incorporate temporal or video-level information.

## 🧪 Tech Stack

- Python
- TensorFlow / Keras
- Jupyter Notebook

## 📊 Results

The model achieves ~90% validation accuracy on the dataset used in this project. Confidence scores closer to 0.5 indicate higher uncertainty near the decision boundary.

## ✍️ Writing

I wrote an accompanying article based on this project, exploring the role of AI in detecting synthetic media.

👉 Medium post: <a href="https://medium.com/@noeflo8006/is-your-face-next-the-battle-of-ai-vs-ai-3fdb1b7ed188">Is Your Face Next? The Battle of AI vs AI</a>
