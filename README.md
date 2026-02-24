

# Brain Tumor Detection System 🧠

## Project Description
A web-based application that uses deep learning to detect brain tumors from MRI scans. The system classifies into four categories: glioma, meningioma, pituitary, and no tumor.

## About Dataset 📊
**Brain Tumor MRI Classification Dataset — 4-Class Medical Imaging Dataset**

🔗 **Dataset Link**: [Kaggle - Brain Tumor MRI](https://www.kaggle.com/datasets/ujjwalsinha01/brain-tumor-mri)

### Overview
A curated medical imaging dataset containing **7,023 MRI scans** for automatic brain tumor classification. The dataset supports **4 classes**: Glioma, Meningioma, Pituitary, and No Tumor. It is designed for deep learning-based medical image analysis and is used to train a high-accuracy CNN + Vision Transformer + Multi-Agent classification pipeline.

### Dataset Statistics

| Split | Images | Percentage |
|-------|--------|------------|
| Training | 5,712 | 81.3% |
| Testing | 1,311 | 18.7% |
| **Total** | **7,023** | **100%** |

### Class Distribution

| Class | Training | Testing | Overall |
|-------|----------|---------|---------|
| Glioma | 1,321 (23.1%) | 300 (22.9%) | 1,621 (23.1%) |
| Meningioma | 1,339 (23.4%) | 306 (23.3%) | 1,645 (23.4%) |
| No Tumor | 1,595 (27.9%) | 405 (30.9%) | 2,000 (28.5%) |
| Pituitary | 1,457 (25.5%) | 300 (22.9%) | 1,757 (25.0%) |

## Features ✨
- **Instant Analysis**: Immediate results upon MRI scan upload
- **High Accuracy**: Utilizes advanced deep learning model
- **User-Friendly Interface**: Simple and interactive UI
- **Real-Time Preview**: Instant preview of uploaded images
- **Reliable Results**: Confidence score with each prediction

## Tech Stack 🛠️
- **Frontend**: HTML, CSS, JavaScript, Bootstrap
- **Backend**: Flask, Streamlit (Python)
- **Deep Learning**: TensorFlow / Keras
- **Image Processing**: PIL, NumPy
- **Model Hosting**: Google Drive (auto-download via gdown)
- **Deployment**: Render

## Installation & Setup 🚀

### 1. Create Virtual Environment
```bash
python -m venv venv
```

### 2. Activate Environment
```bash
# Windows (PowerShell)
.\venv\Scripts\Activate.ps1

# Linux/Mac
source venv/bin/activate
```

### 3. Install Dependencies
```bash
pip install -r requirements.txt
```

### requirements.txt
```
tensorflow
numpy
Pillow
flask
gunicorn
gdown
streamlit
```

### 4. Download the Model
The trained model file (`best_model.keras`, ~227 MB) is hosted on Google Drive. It will be **auto-downloaded** when you run the app for the first time.

If you prefer to download it manually:

📥 **[Download Model from Google Drive](https://drive.google.com/file/d/1aEc1Ni1mds5anu28giaiXkcM9_OOxV2y/view?usp=drive_link)**

After downloading, place the `best_model.keras` file in the project root directory (`Brain-Tumor-Detection-using-CNN/`).

### 5. Run Locally
```bash
# Flask App
python app.py

# Streamlit App
streamlit run streamlit_app.py
```

## Project Structure 📁
```
Brain-Tumor-Detection-using-CNN/
├── app.py                  # Flask web application
├── streamlit_app.py        # Streamlit web application
├── setup.py                # Package setup
├── requirements.txt        # Python dependencies
├── best_model.keras        # Trained model (auto-downloaded via gdown)
├── Brain_tumor_99.ipynb    # Model training notebook
├── samples/                # Sample MRI images for testing
│   ├── glioma/
│   ├── meningioma/
│   ├── notumor/
│   └── pituitary/
├── static/
│   ├── css/
│   │   └── sytle.css
│   ├── js/
│   │   └── main.js
│   └── images/
├── templates/
│   └── index.html
└── README.md
```

## Usage 💡
1. Visit the website
2. Click "Upload" button or drag-and-drop an image
3. Click "Predict" button
4. View results and confidence score

## Deployment 🌐
This application is hosted on Render. For deployment:
- Create a new web service on Render
- Connect GitHub repository
- Build Command: `pip install -r requirements.txt`
- Start Command: `gunicorn app:app`

## Developer 👨‍💻
**Vaibhav Patil**
- [LinkedIn](https://www.linkedin.com/in/vaibhav-patil-654783271)
- [GitHub](https://github.com/12patil)

## License 📝
This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

---

### Note
This project is for educational purposes only and should not be used as the sole tool for medical diagnosis.

## Contributing 🤝
Contributions are welcome! Please feel free to submit a Pull Request.

## Acknowledgments 🙏
- Thanks to all contributors who helped in building this project
- Special thanks to the medical imaging community for providing datasets
- Inspired by the need for accessible medical diagnostic tools

## Support 📧
For support, create an issue in the repository.

