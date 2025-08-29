# Defense-Against-Adversarial-Attacks

## 📌 Problem Statement
Deep Neural Networks (DNNs) have shown exceptional success in solving complex tasks such as image classification, speech recognition, and autonomous systems. However, they are highly vulnerable to **adversarial attacks**, where imperceptible perturbations to input data can cause misclassification and drastically reduce model accuracy.  

This project aims to:
- Study the **nature and behavior** of common adversarial attacks.
- Analyze **defense mechanisms** that can improve model robustness.
- Perform a **comparative study** of attacks and defenses on standard datasets (MNIST, CIFAR10) and a **custom dataset**.

---

## 🎯 Objectives
- Implement and evaluate adversarial attacks:
  - FGSM (Fast Gradient Sign Method)  
  - IFGSM (Iterative FGSM)  
  - MIFGSM (Momentum Iterative FGSM)  
- Study defense mechanisms:
  - Adversarial Training  
  - Defensive Distillation  
- Compare performance on:
  - MNIST (handwritten digits, 10 classes)  
  - CIFAR10 (color images, 10 classes)  
  - Custom dataset (1000 images, 5 classes: flowers, toys, watches, dogs, leaves)

---

## 🏗️ Methodology
1. **Model Training**
   - A CNN model is trained on clean datasets.
   - Baseline accuracy is recorded.

2. **Attack Phase**
   - Perturbations are added to generate adversarial examples.
   - Attacks are performed using FGSM, IFGSM, and MIFGSM.

3. **Defense Phase**
   - Apply adversarial training by retraining with adversarial examples.
   - Apply defensive distillation to reduce model vulnerability.
   - Evaluate post-defense accuracy.

---

## Attack Phase


## 📊 Results
- **Adversarial attacks** reduced model accuracy by more than **70%** on certain datasets.  
- **Adversarial Training** proved to be more effective than Defensive Distillation:
  - On MNIST (FGSM):  
    - Before Attack: **98.21%**  
    - After Attack: **20.40%**  
    - After Defense: **81.93%**
  - On CIFAR10:  
    - Before Attack: **85.54%**  
    - After Attack: **31.84%**  
    - After Defense: **78.16%**
- **Custom Dataset (FGSM)**:  
  - Before Attack: **84.12%**  
  - After Attack: **34.27%**  
  - After Defense: **78.73%**

---
