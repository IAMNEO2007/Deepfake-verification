# 🧠 Deepfake & Fact Verification Platform

A modern Streamlit-based web application designed to analyze media authenticity and verify textual claims. The platform provides a user-friendly interface to upload images, videos, audio, or text documents and returns analysis reports.

## 🚀 Features

*   **Image Authenticity Analysis**: Performs pixel variance and basic analysis to estimate the authenticity of uploaded images, providing an Authenticity Score and a Risk Level (Low, Medium, or High Risk).
*   **Media Support**: Prepared to accept upload formats for Images, Videos, Audio, and Text (`.jpg`, `.jpeg`, `.png`, `.mp4`, `.mp3`, `.wav`, `.txt`).
*   **Text Fact-Checking**: Integrates with Google's Fact Check Tools API to cross-reference claims in uploaded text documents with verified databases.
*   **Verification Reports**: Generates downloadable PDF/Text summary reports detailing authenticity score metrics and risk levels.

---

## 🛠️ Tech Stack

*   **Frontend & UI**: [Streamlit](https://streamlit.io/)
*   **Computer Vision & Image Processing**: [OpenCV (opencv-python-headless)](https://opencv.org/), [Pillow (PIL)](https://python-pillow.org/), [NumPy](https://numpy.org/)
*   **APIs & Networking**: [Requests](https://requests.readthedocs.io/)

---

## 💻 Local Setup & Installation

Follow these steps to run the project locally on your machine:

### 1. Clone the Repository
```bash
git clone https://github.com/IAMNEO2007/Deepfake-verification.git
cd Deepfake-verification
```

### 2. Set Up a Virtual Environment (Recommended)
```bash
# Create a virtual environment
python -m venv venv

# Activate it (Windows PowerShell)
.\venv\Scripts\Activate.ps1

# Activate it (Mac/Linux)
source venv/bin/activate
```

### 3. Install Dependencies
```bash
pip install -r requirements.txt
```

### 4. Set Up Secrets (Optional)
If you want to use the Fact Check API feature, create a `.streamlit/secrets.toml` file in the project root:
```toml
FACT_CHECK_API_KEY = "YOUR_GOOGLE_FACT_CHECK_API_KEY"
```

### 5. Launch the Streamlit App
```bash
streamlit run streamlit_app.py
```
The application will open automatically in your browser at `http://localhost:8501`.
