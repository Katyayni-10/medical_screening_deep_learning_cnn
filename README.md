
# Medical Imaging & Signal Classification — Deep Learning (CNN)

A collection of deep learning projects applying Convolutional Neural Networks (CNNs) to medical imaging and signal classification across four domains: **brain (MRI)**, **eye (fundus imaging)**, **chest (X-ray)**, and **EEG (signal-based)**.

> ⚠️ **Datasets are not included in this repo** due to size (several GB each). Each was sourced from Kaggle — see links below to download and reproduce.

## 📁 Repository Structure

```
medical-imaging-cnn/
├── brain_tumor_classification/
│   ├── model.h5 / model.pt      # trained CNN weights
│   ├── app.py                    # Streamlit app
│   ├── train.py                  # training script
│   └── README.md
├── eye_disease_classification/
├── chest_pneumonia_detection/
├── eeg_seizure_detection/
└── README.md                     # you are here
```

---

## 🧠 Brain — Tumor Classification (4-class)

| | |
|---|---|
| **Task** | Classify brain MRI scans into 4 categories |
| **Classes** | Glioma, Meningioma, Pituitary Tumor, No Tumor |
| **Model** | CNN |
| **Dataset** | Kaggle — [Brain Tumor MRI Dataset](https://www.kaggle.com/datasets/masoudnickparvar/brain-tumor-mri-dataset) |

## 👁️ Eye — Disease Classification (4-class)

| | |
|---|---|
| **Task** | Classify retinal fundus images into 4 categories |
| **Classes** | Normal, Cataract, Diabetic Retinopathy, Glaucoma |
| **Model** | CNN |
| **Dataset** | Kaggle — [Eye Diseases Classification](https://www.kaggle.com/datasets/gunavenkatdoddi/eye-diseases-classification) |

## 🫁 Chest — Pneumonia Detection (binary)

| | |
|---|---|
| **Task** | Classify chest X-rays as Pneumonia or Normal |
| **Classes** | Pneumonia, Normal |
| **Model** | CNN |
| **Dataset** | Kaggle — [Chest X-Ray Images (Pneumonia)](https://www.kaggle.com/datasets/paultimothymooney/chest-xray-pneumonia) |

## 🧬 EEG — Seizure Detection (binary/multi-class)

| | |
|---|---|
| **Task** | Classify EEG signal segments as Seizure or Non-Seizure |
| **Classes** | Seizure, Non-Seizure |
| **Model** | CNN (1D, on signal data) |
| **Dataset** | Kaggle — [Epileptic Seizure Recognition Dataset](https://www.kaggle.com/datasets/harunshimanto/epileptic-seizure-recognition) |

---

## 🛠️ How to Reproduce

```bash
cd project-name/
pip install -r requirements.txt

# 1. Download the dataset from the Kaggle link above and place it in data/
#    (or use the Kaggle API: kaggle datasets download -d <dataset-slug>)

# 2. Train (optional — pretrained weights already included)
python train.py

# 3. Run the Streamlit demo
streamlit run app.py
```

## 📌 Notes

- Trained model weights are included per project (where under GitHub's file size limits); for larger weight files, see the project's own README for a download link (Hugging Face / Releases).
- All datasets are publicly available on Kaggle under their respective licenses — please review each dataset's license/terms before reuse.

## 📫 Contact

Feel free to reach out via [your email / LinkedIn / GitHub profile link] for questions or collaboration.
