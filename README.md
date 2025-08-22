# 🩺 Pneumonia Detection Using CNN & ResNet-18  

> 🚀 Deep Learning project to classify chest X-rays into **Normal** and **Pneumonia** cases, with a focus on **balanced performance** and **explainability**.  

---

## 📌 Project Overview  
Pneumonia remains a major global health issue 🌍, and chest X-ray interpretation can be challenging even for radiologists.  
This project applies **Deep Learning** to assist in Pneumonia detection using **Convolutional Neural Networks (CNNs)** and **ResNet-18**.  

- ✅ **Baseline CNN model** → worked but struggled with **low recall** on Normal cases.  
- ⚡ **Improved with ResNet-18** (transfer learning) → achieved **balanced recall across classes**.  
- 🔎 Added **Grad-CAM visualizations** → so the model’s decision-making becomes **transparent & explainable**.  

---

## 🛠️ Workflow  
1. **Data Preprocessing**  
   - Resized images to standard input size  
   - Normalized pixel intensities  
   - Applied **class weighting** to handle imbalance  

2. **Model Development**  
   - Built a **custom CNN** as baseline  
   - Fine-tuned **ResNet-18** (transfer learning) for improved accuracy  

3. **Evaluation**  
   - Accuracy, Precision, Recall, F1-score  
   - Special focus on **Recall for Normal class**  

4. **Explainability**  
   - Used **Grad-CAM** to highlight regions influencing predictions  
   - Ensured medical interpretability of outputs  

---

## 📊 Results  

| Model        | Accuracy | Recall (Normal) | Recall (Pneumonia) |
|--------------|----------|-----------------|--------------------|
| CNN (baseline) | ~74%    | 0.32            | 0.99               |
| ResNet-18 (fine-tuned) | ~87% | 0.82 | 0.90 |

✨ The ResNet-18 model significantly improved **recall on Normal cases**, making it more reliable in practice.  

---

## 🖼️ Sample Grad-CAM Visualizations  

<p align="center">
  <img src="Grad-CAM Results/Normal Predicted.png" width="45%" />
  <img src="Grad-CAM Results/Normal Predicted.png" width="45%" />
  <img src="Grad-CAM Results/Comparison.png" width="45%" />
</p>  

---

## 📂 Repository Structure  

```
Pneumonia-Detection-CNN-ResNet/
│── README.md
│── requirements.txt
│── Pneumonia_CNN.ipynb
│── Pneumonia_ResNet.ipynb
│── results/
│   ├── training_curve.png
│   ├── gradcam_normal.png
│   ├── gradcam_pneumonia.png
│── models/ (optional)
│   ├── resnet18_best.pth
│── utils.py (optional)
```

---

## 🚀 How to Run  

```bash
# Clone the repo
git clone https://github.com/your-username/Pneumonia-Detection-CNN-ResNet.git
cd Pneumonia-Detection-CNN-ResNet

# Install dependencies
pip install -r requirements.txt

# Run the notebook
jupyter notebook Pneumonia_ResNet.ipynb
```

---

## 📖 Dataset  
Dataset used: **Chest X-ray Dataset (Pneumonia vs Normal)**  
- Kaggle link: [Chest X-ray Pneumonia Dataset](https://www.kaggle.com/paultimothymooney/chest-xray-pneumonia)  
- Contains ~5,800 X-ray images across **Normal** and **Pneumonia** categories  

---

## ✨ Key Highlights  
- 🧠 Implemented **baseline CNN** and improved with **ResNet-18**  
- ⚖️ Tackled **class imbalance** using weighted loss  
- 🔎 Incorporated **Grad-CAM** for interpretability  
- 📈 Achieved **balanced recall** for both Normal and Pneumonia classes  

---

## 📌 Future Work  
- Extend to **multiclass classification** (e.g., Tuberculosis, COVID-19).  
- Explore **Vision Transformers (ViTs)** for further improvement.  
- Deploy as a **web app** for clinical usability.  

---

## 👨‍💻 Author  
**Vipul Parmar**  
- 📧 [vipulparmar3018@gmail.com](mailto:vipulparmar3018@gmail.com)  
- 🔗 [LinkedIn](https://www.linkedin.com/in/vipul-parmar-886b48256/) | [GitHub](https://github.com/weepull)  

---
