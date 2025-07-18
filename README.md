# Detecting Antibiotic Resistance in Bacteria from Microscopic Images using Deep Learning

This project demonstrates an end-to-end deep learning pipeline to detect antibiotic resistance in *E. coli* using fluorescence microscopy images.

## 🧠 Technologies Used

- **Python**
- **TensorFlow + Keras** (U-Net for segmentation)
- **scikit-learn** (Random Forest classifier)
- **OpenCV**, **scikit-image**, **Pandas**, **NumPy**
- Google Colab (with NVIDIA T4 GPU)

## 📊 Key Results

- **Segmentation Accuracy**: 99%
- **Classification Accuracy**: 91%
- **Dice Coefficient (IoU)**: 0.88
- **Model Type**: U-Net for segmentation, Random Forest for classification

## 📁 Repository Structure

```bash
📁 segmentation_model/      # U-Net architecture and training
📁 classification_model/    # Morphological features + Random Forest
📁 dataset/                 # Link or sample images (not full dataset)
📁 results/                 # Sample output masks and predictions
📄 AMR_final_report.pdf     # Final B.Tech academic report
📄 requirements.txt         # All dependencies
📄 README.md                # This file
```

## 📚 Dataset

- **Source**: Deep Antimicrobial Susceptibility Phenotyping (DASP), University of Oxford  
- **License**: CC-BY-NC 4.0 International  
- [Link to Dataset](https://doi.org/10.1101/2022.12.08.22283219)

## 📌 How It Works

1. **Image Preprocessing**
   - TIFF image loading, resizing, normalization

2. **Segmentation**
   - U-Net trained on MG1655 strain microscopy images

3. **Feature Extraction**
   - Area, perimeter, eccentricity, solidity, aspect ratio, intensity metrics

4. **Classification**
   - Random Forest trained on features to classify cells as Resistant or Susceptible

## 🧪 Testing and Evaluation

- Confusion Matrix, ROC, Precision-Recall curves
- Hyperparameter tuning via RandomizedSearchCV

## ✍️ Authors

- C G Harsha Vardhan (BU21CSEN0100917)  
- B Ramprasad (BU21CSEN0100932)  
- L Nidhi (BU21CSEN0102047)

## 📄 License

This project is for academic purposes only and uses datasets under the [CC-BY-NC 4.0 License](https://creativecommons.org/licenses/by-nc/4.0/).
