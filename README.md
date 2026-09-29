# AI Attention Visualizer

An interactive AI application that visualizes how an attention-based model processes and represents text. The project uses sentence embeddings to analyze text and provides a simple visual interface through Streamlit.

## Features

* Generate sentence embeddings using `all-MiniLM-L6-v2`
* Compare text using embedding similarity
* Visualize attention/representation-related information
* Interactive Streamlit interface
* Simple and beginner-friendly UI
* Uses Hugging Face Sentence Transformers
* Fast semantic text comparison

## Technologies Used

* **Python**
* **Streamlit**
* **Sentence Transformers**
* **NumPy**
* **Pillow**
* **PyTesseract**
* **Hugging Face**
* **Scikit-learn / Cosine Similarity**

## Project Structure

```text
AI Attention Visualizer/
│
├── app.py
├── embedding.py
├── requirements.txt
├── README.md
└── venv/
```

> `venv/` should not be uploaded to GitHub. Add it to `.gitignore`.

## Installation

### 1. Clone the repository

```bash
git clone https://github.com/your-username/AI-Attention-Visualizer.git
cd AI-Attention-Visualizer
```

### 2. Create a virtual environment

```bash
python -m venv venv
```

### 3. Activate the virtual environment

**Windows PowerShell:**

```powershell
.\venv\Scripts\Activate.ps1
```

### 4. Install dependencies

```bash
python -m pip install -r requirements.txt
```

If `requirements.txt` is not available, install the main packages manually:

```bash
python -m pip install streamlit numpy pillow pytesseract sentence-transformers
```

## Run the Application

Start the Streamlit application using:

```bash
streamlit run app.py
```

The application will open in your browser.

## How It Works

The application follows a simple workflow:

```text
User Input
    ↓
Text Processing
    ↓
Sentence Transformer
    ↓
Embedding Generation
    ↓
Similarity / Attention Analysis
    ↓
Visualization
```

The `all-MiniLM-L6-v2` model converts text into numerical vector representations called **embeddings**. These embeddings can then be compared to understand the semantic relationship between pieces of text.

## Example

Input:

```text
Artificial Intelligence is changing education.
AI is transforming the way students learn.
```

The application converts both sentences into embeddings and analyzes their semantic similarity.

## Requirements

* Python 3.10+
* Internet connection for the first model download
* Streamlit
* Sentence Transformers
* NumPy
* Pillow
* PyTesseract

## Important Note

The first time the application runs, `all-MiniLM-L6-v2` may need to be downloaded from Hugging Face. Therefore, an internet connection is required during the initial setup.

If Hugging Face connection errors occur, try:

```powershell
$env:HF_HUB_DISABLE_XET="1"
```

Then run the application again.

## Future Improvements

* Add interactive attention heatmaps
* Add token-level visualization
* Support image and document input
* Add multiple embedding models
* Add downloadable visualization reports
* Improve UI and customization
* Add real-time comparison between multiple texts

## Learning Objectives

This project demonstrates:

* Natural Language Processing
* Text embeddings
* Transformer models
* Semantic similarity
* Attention concepts
* Streamlit application development
* Hugging Face model integration
