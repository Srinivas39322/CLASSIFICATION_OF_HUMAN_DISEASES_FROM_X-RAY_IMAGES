### Classification of Human Diseases from X-Ray Images 🌐📷

---

#### **Introduction**
This project utilizes deep learning to classify chest X-ray images into four categories: Pneumonia, COVID-19, Tuberculosis, and Normal. By employing the ResNet50 convolutional neural network architecture, the model aims to enhance diagnostic accuracy in medical imaging through advanced feature extraction and classification techniques.

---

#### **Objective**
To develop a convolutional neural network (CNN) model using ResNet50 to classify chest X-ray images into disease categories, improving diagnostic support and enabling early detection of critical illnesses.

---

#### **SMART Questions**
1. How effectively can ResNet50 classify X-ray images into distinct disease categories?
2. Does balancing the dataset improve classification accuracy for underrepresented classes?
3. How does the model’s performance change with the inclusion of BatchNormalization and Dropout layers?
4. What metrics best represent the success of the classification model (e.g., accuracy, loss)?
5. Can the model achieve a high generalization capability across diverse datasets?

---

#### **Dataset**
- **Source**: [Kaggle Chest X-Ray Dataset](https://www.kaggle.com/)
- **Size**: 6326 images
- **Categories**:
  - Pneumonia
  - COVID-19
  - Tuberculosis
  - Normal
- **Structure**: Training, validation, and test sets with augmented image data.

---

#### **Key Findings/Conclusion**
1. **Model Performance**:
   - Initial accuracy: 74% with a loss of 0.6596 (underfitting observed).
   - Balanced dataset accuracy: Improved to 81% with a loss of 0.4910.

2. **Model Enhancements**:
   - BatchNormalization stabilized and accelerated training.
   - Dropout layers reduced overfitting by deactivating 50% of neurons randomly during training.

3. **Dataset Observations**:
   - Unbalanced dataset with an overrepresentation of Pneumonia images.
   - Implementing `compute_class_weight` improved fairness and performance.

4. **Conclusion**:
   - ResNet50, with fine-tuning and proper balancing techniques, demonstrates strong performance in disease classification.
   - Incorporating balanced data and advanced techniques such as BatchNormalization is critical for improving model efficiency and reliability.

---
