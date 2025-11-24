Project Title: Comparative Study of Custom CNN and Transfer Learning for Banana Leaf Disease Classification

Overview: This project compares a Custom Convolutional Neural Network (CNN) and a Transfer Learning model (VGG16) to classify banana leaf diseases.  
The dataset used includes four classes Cordana, Fresh (Healthy), Pestalotiopsis and Sigatoka sourced from Mendeley Data.  
Both models were trained with and without Early Stopping to evaluate performance, overfitting, and generalization on a small dataset.

Dataset:
Source: https://data.mendeley.com/datasets/wfzpdmc5vx/1
Structure: 4 folders (one per class) 
Total Images: 423  

Results Summary:

| Model       | Early Stopping | Training Accuracy | Validation Accuracy | Validation Loss |
|--------------|----------------|------------------:|--------------------:|----------------:|
| Custom CNN   | No             | 0.55              | 0.28                | 18.5            |
| Custom CNN   | Yes            | 0.70              | 0.60                | 1.20            |
| VGG16        | No             | 0.82              | 0.80                | 0.65            |
| VGG16        | Yes            | 0.88              | 0.81                | 0.50            |
                   
Among all tested models VGG16 with Early Stopping demonstrated the best overall performance achieving the highest validation accuracy of 81% with the lowest validation loss of 0.50.  
This clearly indicates that transfer learning using VGG16 is far more effective than the Custom CNN for small datasets.  
The Custom CNN though efficient and lightweight struggled with overfitting and limited generalization due to the small dataset size. Early Stopping improved its performance slightly, but it still remained below VGG16 in terms of stability, precision, and recall.
