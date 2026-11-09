# Evaluation of Computer Vision Models

## 📌 Description

Ce projet présente l'évaluation de plusieurs modèles de **Computer Vision** déjà entraînés. L'objectif est de comprendre comment évaluer les performances des modèles selon différentes tâches de vision par ordinateur.

Le projet couvre trois tâches principales :

- **Object Detection**
- **Semantic Segmentation**
- **Instance Segmentation**

> Les modèles utilisés sont déjà pré-entraînés. Aucun entraînement de modèle n'est réalisé dans ce projet.

---

## 🤖 Modèles utilisés

| Tâche | Modèle |
|---|---|
| Object Detection | Faster R-CNN |
| Semantic Segmentation | DeepLabV3 |
| Instance Segmentation | Mask R-CNN |

---

## 📊 Métriques d'évaluation

Les performances des modèles sont évaluées à l'aide de plusieurs métriques :

- **IoU (Intersection over Union)** : mesure le chevauchement entre la prédiction et la Ground Truth.
- **Precision** : mesure la proportion des prédictions correctes.
- **Recall** : mesure la capacité du modèle à détecter les objets existants.
- **mAP (mean Average Precision)** : mesure globale des performances en détection d'objets.
- **Pixel Accuracy** : mesure le pourcentage de pixels correctement classifiés.
- **mIoU (mean Intersection over Union)** : moyenne de l'IoU sur les différentes classes.
- **Dice Score** : mesure la similarité entre les masques prédits et les masques réels.

---

## 📁 Dataset

Le projet utilise le dataset **COCO (val2017)**.

Les annotations du dataset contiennent les informations nécessaires pour construire la **Ground Truth**, notamment :

- Les classes des objets
- Les bounding boxes
- Les masques de segmentation

---

## 🛠️ Technologies utilisées

- Python
- PyTorch
- Torchvision
- NumPy
- Pandas
- Matplotlib
- PyCOCOTools
- TorchMetrics

---

## 🚀 Exécution

Le notebook peut être exécuté dans **Google Colab** ou dans un environnement Python disposant des bibliothèques nécessaires.

Installez les dépendances principales :

```bash
pip install pycocotools torchmetrics
```

Ensuite, ouvrez et exécutez le notebook :

```text
Evaluation_Computer_Vision_Models.ipynb
```

---

## 📚 Contenu du projet

Le notebook est organisé en trois parties :

### 1. Object Detection

Utilisation du modèle **Faster R-CNN** pour détecter les objets dans les images à l'aide de bounding boxes.

Métriques principales :

- IoU
- Precision
- Recall
- mAP

### 2. Semantic Segmentation

Utilisation du modèle **DeepLabV3** pour attribuer une classe à chaque pixel de l'image.

Métriques principales :

- Pixel Accuracy
- IoU / mIoU
- Dice Score

### 3. Instance Segmentation

Utilisation du modèle **Mask R-CNN** pour détecter chaque objet et générer un masque pour chaque instance.

Métriques principales :

- IoU des masques
- Dice Score
- Mask mAP

---

## 🎓 Contexte académique

Projet réalisé dans le cadre d'un travail sur l'**évaluation des modèles de Computer Vision**.

**Groupe 1**  
Thèmes : Object Detection, Semantic Segmentation et Instance Segmentation.
