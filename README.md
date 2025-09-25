# Restrictive-Breed-Classifier  

**Deep Learning for Restricted Dog Breed Identification**  

This project develops and evaluates deep learning models for the classification of dog breeds restricted under Irish law. It explores transfer learning with frozen convolutional bases, batch normalization, dropout regularisation, and fine-tuning strategies.  

## Key Features  
- **Transfer Learning on ImageNet:** Six pretrained CNN architectures benchmarked:  
  - VGG16  
  - ResNet50  
  - InceptionV3  
  - Xception  
  - InceptionResNetV2  
  - NASNetMobile  
- **Model Selection:** Best performers (NASNetMobile, InceptionResNetV2) fine-tuned by unfreezing top convolutional layers.  
- **Ensemble Approach:** Combined predictions of top models to improve robustness.  
- **Performance:**  
  - Accuracy: **97.05%**  
  - Precision: **99.09%**  
  - F1-score: **98%+**  
- **Interpretability:** Grad-CAM heatmaps used to verify model focus on breed-specific features.  
- **Reproducible Pipeline:** Balanced restricted vs. unrestricted dataset, fixed seed, and consistent data splits.  

## Motivation  
Breed-specific legislation (BSL) in Ireland regulates or prohibits ownership of certain breeds. Enforcement often relies on subjective human judgement, leading to misclassification, legal disputes, and welfare concerns. This project demonstrates how CNNs can assist by providing **objective, reproducible, and interpretable** breed classification.  

## Outputs  
- Training and validation learning curves for all models  
- Confusion matrices with counts and percentages  
- Grad-CAM overlays for interpretability  
- Saved Keras models and weights for deployment  
