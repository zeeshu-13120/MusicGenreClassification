# 🎵 Music Genre Classification

## 📌 Overview
This project aims to classify **music genres** from audio files using the **GTZAN dataset**.  
It explores two distinct machine learning pipelines:  
1. **Traditional Approach** — using handcrafted audio features.  
2. **Deep Learning Approach** — using spectrogram images and transfer learning.

The goal is to compare **classical machine learning** with **deep learning** for multi-class classification and evaluate the impact of different feature representations.

---

## 📂 Project Workflow

### **1. Audio Feature Extraction**
- Extracted **MFCCs, spectral centroid, zero-crossing rate, chroma features**, and more.
- Created a **tabular dataset** for classical ML models.

### **2. Spectrogram Generation**
- Converted raw audio into **Mel spectrogram images** for image-based models.

### **3. Model Implementation & Evaluation**
- **Random Forest Classifier** on tabular features.
- **CNN (Convolutional Neural Network)** on spectrograms.
- **Transfer Learning with VGG16** on spectrograms.

### **4. Final Model Selection**
- Compared models based on **accuracy, F1-score, and confusion matrices**.
- Selected the **best-performing model** for deployment.

---

## 📊 Dataset
- **GTZAN Dataset**: 10 genres × 100 audio tracks each = **1000 tracks**.
- Widely used benchmark for **music genre classification**.

**Kaggle Link:** [GTZAN Dataset - Music Genre Classification](https://www.kaggle.com/datasets/andradaolteanu/gtzan-dataset-music-genre-classification)

---

## 🛠 Technologies Used
- **Python 3.12.10**
- **Jupyter Notebook**
- **Pandas** — Data manipulation
- **NumPy** — Numerical operations
- **Librosa** — Audio analysis & feature extraction
- **Scikit-learn** — Preprocessing & classical ML
- **TensorFlow/Keras** — Deep learning models
- **Matplotlib** — Data visualization
- **Seaborn** — Confusion matrices & plots
- **KaggleHub** — Dataset downloading
- **tqdm** — Progress visualization

---

## ⚙ Installation

### **1️⃣ Clone the Repository**
```bash
git clone https://github.com/zeeshu-13120/MusicGenreClassification
cd MusicGenreClassification
```

### **2️⃣ Set Up Virtual Environment**
```bash
# Create virtual environment
python -m venv venv

# Activate it (Windows)
.venv\Scripts\activate

# Activate it (macOS/Linux)
source venv/bin/activate
```

### **3️⃣ Install Dependencies**
```bash
pip install -r requirements.txt
```
> Note: Dataset will be automatically downloaded using **kagglehub**.

### **4️⃣ Launch JupyterLab**
```bash
jupyter-lab
```

---

## 🚀 Usage
1. Open `Music_Genre_Classification.ipynb` in JupyterLab.  
2. Run all cells sequentially.  
3. Explore **model comparison results** at the end of the notebook.

---

## 📂 Project Structure
```
├── Music_Genre_Classification.ipynb    # Main notebook
├── extracted_features.csv              # Tabular dataset of extracted features
├── spectrogram_images/                 # Directory with generated spectrograms
├── requirements.txt                    # Project dependencies
├── README.md                           # Project documentation
├── ProjectReport_Zeeshan.pdf           # Detailed project report
```

---

## 🤝 Contributing
Contributions are welcome!  
- Fork the repository  
- Create a new branch (`feature-branch`)  
- Commit your changes  
- Open a Pull Request  

For major updates, please open an **issue** first to discuss the proposed changes.

---

## 📜 License
This project is licensed under **Unlicense** — free to use without restrictions.

---

📧 **Contact**  
For any inquiries or collaborations, reach out via GitHub Issues or email.
