# Pneumonia Detection Using Deep Learning

This project is focused on building a CNN-based model using FastAI to automatically detect **Pneumonia** from chest X-ray images. It showcases the use of **transfer learning** with **ResNet50** for medical image classification.

---

## Project Structure

```
pneumonia-detection-using-deep-learning/
├── Pneumonia_Detection.ipynb                
├── Pneumonia_Detection_Presentation.pptx 
├── README.md                                 
├── requirements.txt                          
└── dataset/                                  
```

---

## Dataset Details

- 📦 Source: [Chest X-Ray Images (Pneumonia) – Kaggle](https://www.kaggle.com/datasets/paultimothymooney/chest-xray-pneumonia)
- 📂 Categories: `NORMAL`, `PNEUMONIA`
- 🖼️ Format: JPG images in `train/`, `val/`, `test/` folders

*Note: Dataset is not included due to size constraints. Please download it manually.*

---

## Libraries & Tools Used

- Python 3.9+
- FastAI
- PyTorch
- Jupyter Notebook
- NumPy, Pandas, Matplotlib
- PIL (Python Imaging Library)

---

## Model Summary

- Model: Pretrained **ResNet50**
- Image Input Size: 224x224
- Used FastAI's `cnn_learner` with `fit_one_cycle` training
- Loss function: Cross Entropy
- Metric: Accuracy
- GPU Accelerated training

---

## Running the Project

1. Clone the repository:

```bash
git clone https://github.com/yourusername/pneumonia-detection-fastai.git
cd pneumonia-detection-fastai
```

2. Install dependencies:

```bash
pip install -r requirements.txt
```

3. Launch Jupyter Notebook:

```bash
jupyter notebook Pneumonia_Detection.ipynb
```

4. Ensure dataset is in the correct path (`dataset/chest_xray`), or modify the notebook path as needed.

---

## Sample Output

> Model predicts between `NORMAL` and `PNEUMONIA` categories from chest X-rays.

```
Predicted: PNEUMONIA
```

You will also see:
- Confusion matrix
- Learning rate graph
- Sample prediction visualizations

---

## Presentation

This project includes a PowerPoint presentation for academic submission:

[Pneumonia_Detection_Presentation_CA4.pptx](./Pneumonia_Detection_Presentation_CA4.pptx)

---

## Conclusion

We demonstrated that a CNN model using transfer learning with ResNet50 can accurately classify pneumonia from chest X-rays. With further fine-tuning and more data, such models can assist in faster and more accessible diagnosis in healthcare.

---

## Acknowledgements

- [FastAI Library](https://www.fast.ai/)
- [PyTorch](https://pytorch.org/)
- [Paul Mooney's Dataset on Kaggle](https://www.kaggle.com/datasets/paultimothymooney/chest-xray-pneumonia)
- Project prepared for: *Deep Learning Applications - AI & Data Analytics*

---

> For feedback or collaboration, feel free to fork this repo or raise an issue.
