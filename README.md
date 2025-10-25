# 🦾 Animal Image Classifier using Vision Transformer (ViT)

This project is a **deep learning application** that classifies **animal images** using the **Vision Transformer (ViT)** model — an advanced alternative to traditional CNN architectures.  
The model was trained with **transfer learning** and **fine-tuning** techniques, achieving **high accuracy** in animal species prediction.

---

## 🌍 Overview

A **ViT-based model** utilizing a **global attention mechanism** as an alternative to conventional CNNs.  
This project leverages **PyTorch**, **OpenCV**, and **Gradio** to provide a complete and interactive image classification system.

---

## ✨ Features

- 🧠 **Modern Architecture**: Uses **Vision Transformer (ViT-B-16)** — one of the most advanced models for image classification.  
- 📊 **High Performance**: Achieved **~97% accuracy** on the validation dataset.  
- 🎨 **Advanced Preprocessing**: Improves input quality with **Denoising**, **Sharpening**, and **CLAHE (Contrast Enhancement)** using OpenCV.  
- 💻 **Interactive Interface**: Provides a simple, fast, and user-friendly **web UI** built with **Gradio**.  

---

## 🧰 Technologies Used

| Technology | Purpose |
|-------------|----------|
| 🐍 **PyTorch & Torchvision** | Building, training, and loading the ViT model |
| ⚙️ **Gradio** | Rapid prototyping and web-based interface |
| 🧩 **OpenCV (cv2)** | Image preprocessing (denoise, sharpen, CLAHE) |
| 🧮 **NumPy & PIL** | Image manipulation and array handling |

---

## ⚙️ Setup and Launch

Follow these steps to run the project on your local machine 🖥️

### 1️⃣ Clone the Repository
```bash
git clone https://github.com/CuneytBaskurt/Animal-Image-Classifier.git
cd Animal-Image-Classifier
```
```bash
2️⃣ Install Requirements
pip install torch torchvision gradio opencv-python numpy pillow
```
```bash
3️⃣ Download Model and Dataset
Due to the large size of files, the model weights and dataset are hosted on Google Drive.

🔽 Model Weights (vit_model.pth)

📁 Download Model from Google Drive

Action: Place the vit_model.pth file in the project’s root directory (next to the script file).

📦 Dataset (Required for Script)

📁 Download Dataset from Google Drive

Action: The provided script reads class names from this dataset.
```

🖼️ Model & Preprocessing Pipeline

Before classification, several filters are applied to enhance image quality — improving prediction accuracy even on low-quality or noisy images.

| Step                                | Description                                  |
| ----------------------------------- | -------------------------------------------- |
| 🧹 **Denoising**                    | Removes random pixel noise                   |
| ✨ **Sharpening**                    | Enhances edges and fine details              |
| 🌗 **Contrast Enhancement (CLAHE)** | Highlights details in dark or bright regions |

After these enhancements, the filtered image is sent to the ViT model, and the Top-5 predictions with their probabilities are displayed to the user.

🚀 Example Workflow

1. Upload or drag an animal image 🐯

2. The image is automatically preprocessed (denoised, sharpened, CLAHE)

3. ViT model classifies the image and returns top 5 predictions

4. Results are displayed instantly via Gradio interface

🧑‍💻 Author

Cüneyt Oğuz Başkurt
📍 Computer Engineering Student — Kocaeli University
🔗 GitHub Profile

