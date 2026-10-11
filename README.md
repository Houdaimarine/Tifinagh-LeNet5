# Tifinagh-LeNet5
# ⵣ Tifinagh Handwritten Character Recognition using Modified LeNet-5

[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/Houdaimarine/Tifinagh-LeNet5/blob/main/Tifinagh_LeNet5_Training.ipynb)

Ce projet implémente un système de reconnaissance automatique des caractères manuscrits de l'alphabet amazigh (**Tifinagh**) en utilisant une architecture de Réseau de Neurones Convolutif (CNN) inspirée et modifiée du modèle historique **LeNet-5**.

---

##  À Propos du Projet
* **Dataset :** [AMHCD (Amazigh Handwritten Character Database)](https://www.kaggle.com/datasets/benaddym/amazigh-handwritten-character-database-amhcd) contenant 25 740 images au total (20 592 pour l'entraînement et 5 148 pour la validation) réparties sur **33 classes**.
* **Modèle :** LeNet-5 Modifié (Implémenté en PyTorch).
* **Performance :** Précision de validation atteinte : **93.40%** après 5 époques.
* **Environnement :** Google Colab avec GPU (NVIDIA T4).

---

##  Structure de l'Architecture
Le modèle s'appuie sur la séquence de couches suivante :
1. **C1 (Convolution)** : 6 filtres ($5 \times 5$) + ReLU
2. **S2 (Pooling Moyen)** : $2 \times 2$
3. **C3 (Convolution)** : 16 filtres ($5 \times 5$) + ReLU
4. **S4 (Pooling Moyen)** : $2 \times 2$
5. **C5 & F6 (Fully Connected)** : Couches denses de 120 et 84 neurones.
6. **Sortie (Output)** : 33 classes (logits).

---

##  Comment Exécuter le Projet ?
Vous pouvez lancer et tester directement l'entraînement et l'évaluation du modèle sur Google Colab en cliquant sur le badge ci-dessus :  
 **[Ouvrir le Notebook dans Google Colab](https://colab.research.google.com/github/Houdaimarine/Tifinagh-LeNet5/blob/main/Tifinagh_LeNet5_Training.ipynb)**

---

##  Résultats Clés
* **Courbes d'Apprentissage :** Diminution stable de la perte (Loss) et augmentation de la précision (Accuracy).
* **Matrice de Confusion :** Bonne séparabilité des 33 classes de caractères Tifinagh.
* **Feature Maps :** Visualisation de l'extraction des contours géométriques par la couche C1.

---

## 📄 Rapport du Projet (Article Scientifique)
Le rapport complet rédigé en LaTeX (format article académique IMRAD) décrivant l'ensemble de la méthodologie, l'architecture du réseau, et l'analyse des résultats est disponible ici :
* 📥 **[Télécharger / Lire le Rapport PDF (Article)](./ARTICLE_deep_learning.pdf)**

##  Auteur
* **Houda Imarine**  
  *Université Ibn Zohr, Faculté Polydisciplinaire d'Ouarzazate*  
  *Master Intelligence Artificielle et Applications*
