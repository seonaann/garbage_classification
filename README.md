# 🗑️ Garbage Classification using EfficientNetV2B2

A deep learning model for classifying waste images into six categories using transfer learning with EfficientNetV2B2.  
Built with TensorFlow & Keras and deployed via Gradio on Hugging Face Spaces.

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

👉 Try the deployed model here: [Garbage Classifier on Hugging Face](https://huggingface.co/spaces/seonaann/garbage-classifier)

---

## 📊 Model Performance

| Metric        | Value   |
|---------------|---------|
| ✅ Accuracy    | 92.97%  |
| 📉 Test Loss   | 0.2643  |

> 📌 The model performs exceptionally well on all classes except **“trash”**, which is underrepresented and visually ambiguous.

---

## 🧠 How It Works

- 📁 Dataset loaded from TrashNet (resized & preprocessed)  
- 🔍 Data Augmentation: Flip, Zoom, Contrast, Rotation  
- ⚖️ Class balancing using computed weights  
- 🧠 Model: EfficientNetV2B2 with top layers replaced  
- 🧪 Training: Fine-tuned with EarlyStopping + ReduceLROnPlateau

---

## 🛠️ Tech Stack

- TensorFlow / Keras  
- EfficientNetV2B2 (ImageNet pretrained)  
- Gradio (web deployment)  
- Hugging Face Spaces  
- Python, NumPy, PIL

---

## 🧪 Sample Predictions

| Example Image      | Predicted Class | Confidence |
|--------------------|------------------|------------|
| Plastic bottle      | Plastic          | 0.93       |
| Paper sheet         | Paper            | 0.91       |
| Metal can           | Metal            | 0.89       |
| Trash mix (wrong)   | Paper ❌         | 0.61       |

> ⚠️ *Note: The “trash” class has lower accuracy due to fewer examples and overlap with other categories.*

---

## 📁 Project Structure

```bash
garbage-classification/
├── app.py                        # Gradio interface
├── EfficientNetV2B2_model.keras  # Trained model
├── requirements.txt              # Dependencies
└── README.md                     # This file


👉 Try the live app on Hugging Face

🧑‍💻 Author
Made with ❤️ by Seona Ann Tom
🔗 GitHub: @seonaann

📜 License
This project is licensed under the MIT License.

🙌 Acknowledgements
Dataset inspired by TrashNet

Hugging Face for free model hosting via Spaces

Gradio for the fast, no-code interface
