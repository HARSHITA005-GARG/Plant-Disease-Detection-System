<h1>🌱 Plant Disease Detection System </h1> 

<p align="center">
  <img src="https://img.shields.io/badge/Python-3.8%2B-blue?style=flat-square">
  <img src="https://img.shields.io/badge/Deep%20Learning-CNN-green?style=flat-square">
  <img src="https://img.shields.io/badge/License-MIT-yellow?style=flat-square">
</p>

A Streamlit-based web application for automated plant disease detection using Deep Learning. This system helps farmers and agricultural professionals identify plant diseases early, supporting sustainable farming practices and reducing crop losses.

![image](https://github.com/user-attachments/assets/af06dabc-2a23-4761-b9b6-c56ddc7cdc16)
![image](https://github.com/user-attachments/assets/755c6dc7-d851-475b-9602-7a00d210656b)
![image](https://github.com/user-attachments/assets/20e2c937-f581-41a5-b42c-02e2e64d4a45) ![image](https://github.com/user-attachments/assets/742d290a-5188-4812-a538-ce696f022d8c)
![image](https://github.com/user-attachments/assets/5be172c5-8d66-4b46-b657-1ab5ea43ccf1)


## 🌟 Features

- 🖼️ Image-based disease detection using CNN
- 📊 Real-time classification results with confidence scores
- 🌿 Support for multiple plant species
- 📝 Detailed disease information and treatment recommendations
- 🌍 Sustainability-focused design for eco-friendly agriculture

## 🛠️ Prerequisites

- Python 3.8+
- pip package manager
- Virtual environment (recommended)

## ⚙️ Installation

1. Clone the repository:
```bash
git clone https://github.com/HARSHITA005-GARG/Plant-Disease-Detection-System.git
cd Plant-Disease-Detection-System
```

2. Create and activate virtual environment:
```bash
python -m venv venv
source venv/bin/activate  # Linux/MacOS
venv\Scripts\activate  # Windows
```

3. Install dependencies:
```bash
pip install -r requirements.txt
```

## 🚀 Usage

1. Start the Streamlit application:
```bash
streamlit run app.py
```

2. In the web interface:
 - Click "Browse files" to upload a plant image
 - Wait for the model prediction (typically 2-5 seconds)
 - View disease diagnosis and recommended actions

## 🧠 Model Architecture

The CNN architecture consists of:
```python
model = Sequential([
    Conv2D(32, (3,3), activation='relu', input_shape=(224,224,3)),
    MaxPooling2D(2,2),
    Conv2D(64, (3,3), activation='relu'),
    MaxPooling2D(2,2),
    Dropout(0.25),
    Flatten(),
    Dense(128, activation='relu'),
    Dense(num_classes, activation='softmax')
])
```

## 🤝 Contributing

1. Fork the repository
2. Create your feature branch:
```bash
git checkout -b feature/your-feature-name
```
3. Commit your changes
4. Push to the branch
5. Open a Pull Request

## 📜 License
Distributed under the MIT License. See `LICENSE` for more information.

## 🙏 Acknowledgements
- PlantVillage Dataset
- Streamlit Community
- TensorFlow/Keras Documentation
