# 🗑️ Garbage Classification using EfficientNetV2B2

A deep learning model for classifying waste images into six categories using transfer learning with EfficientNetV2B2.  
Built with TensorFlow & Keras and deployed via Gradio.

---

## 📌 Categories

The model can classify images into the following categories:

- 📦 Cardboard  
- 🔮 Glass  
- ⚙️ Metal  
- 📄 Paper  
- 🧴 Plastic  
- 🚮 Trash  

---

## 🚀 Live Demo (Hugging Face)

Try the deployed model here:  
👉 **[Garbage Classifier on Hugging Face](https://huggingface.co/spaces/seonaann/garbage-classifier)**

---

## 📊 Model Performance

| Metric        | Value     |
|---------------|-----------|
| ✅ Accuracy    | 92.97%    |
| 📉 Test Loss   | 0.2643    |

The model performs exceptionally well on all classes except "trash", which is underrepresented and visually ambiguous.

---

## 🧠 How It Works

- 📁 Dataset loaded from TrashNet (resized & preprocessed)
- 🔍 Data Augmentation: flip, zoom, contrast, rotation
- ⚖️ Class balancing using computed weights
- 🧠 Model: EfficientNetV2B2 with top layers replaced
- 🧪 Fine-tuned with early stopping + learning rate scheduling

---

## 🛠️ Tech Stack

- **TensorFlow / Keras**
- **EfficientNetV2B2 (ImageNet pretrained)**
- **Gradio** for web deployment
- **Hugging Face Spaces**
- **Python, NumPy, PIL**

---

## 🧪 Sample Predictions

| Example Image            | Predicted Class | Confidence |
|--------------------------|------------------|------------|
| *plastic bottle*         | Plastic          | 0.93       |
| *paper sheet*            | Paper            | 0.91       |
| *metal can*              | Metal            | 0.89       |
| *trash mix (wrong)*      | Paper            | 0.61 ❌    |

> Note: Trash class has lower accuracy due to fewer examples and overlap with other categories.

---

## 📁 Project Structure

📦 garbage-classification/
├── app.py # Gradio interface
├── EfficientNetV2B2_model.keras # Trained model
├── requirements.txt # Dependencies
├── README.md # This file

## 🚀 Live Demo Preview

![Hugging Face Demo](https://github.com/seonaann/garbage_classification/blob/main/hf_demo.png.png)

👉 Try the live app here: [Hugging Face Space](https://huggingface.co/spaces/seonaann/garbage-classifier)


---

## 🧑‍💻 Author

Made with ❤️ by [Seona Ann Tom](https://www.linkedin.com/in/seona-ann-tom-06351332a)  
🔗 GitHub: [@seonaann](https://github.com/seonaann)

---

## 📜 License

This project is licensed under the **MIT License**.

---

## 🙌 Acknowledgements

- Dataset inspired by [TrashNet](https://github.com/garythung/trashnet)
- Hugging Face for free hosting via Spaces
- Gradio for the easy-to-build UI interface


  
