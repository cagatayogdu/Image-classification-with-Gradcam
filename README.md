# A Deep Learning-Based Approach and Heat Map Creation for Damage Detection in Cultural Heritage Images

This project aims to develop a method for detection and analysis using deep learning models on images of damaged and undamaged cultural heritage structures, contributing to the preservation of cultural heritage. Acknowledging the fact that cultural structures can deteriorate over time due to external factors such as natural and social disasters, the project emphasizes the importance of detecting and analyzing damage to these structures.

This work has been published in IEEE. The full paper is available at:
https://doi.org/10.1109/ICSH62408.2024.10779884

## Aim and Methodology
The aim of this project is to develop an effective method for the preservation of cultural heritage. This method aims to identify damaged areas of structures and analyze them visually using deep learning and image processing techniques. This enables a clearer identification and analysis of damaged areas in the image. This method could play an important role in the preservation of cultural heritage by identifying damaged areas and directing them towards restoration.

## Data Set

Our dataset consists of 541 images of damaged and 625 images of undamaged cultural heritage structures. The damaged images are labeled as (1) and the undamaged images as (0). There is no significant imbalance between the number of damaged and undamaged images in the dataset. The difference in the numbers of damaged and undamaged images is sufficient to train the model in a balanced manner.

![image](https://github.com/cagatayogdu/Image-classification-with-Gradcam/assets/160175656/13ee3419-34f6-4bb9-8819-967995f39bff)

Above, as a result of the data augmentation process applied to a cultural heritage image, 9 different images have been obtained.

## Recommended Model

The proposed model has been expanded with various layers to enhance performance and increase the depth of the network beyond these pretrained models. The "Class Activation Mapping Layer" section has been created using the Grad-CAM (Gradient-weighted Class Activation Mapping) method, which is used to explain the visual results of deep neural networks. Heatmaps have been created using the Grad-CAM method for damage detection in cultural heritage sites.

![image](https://github.com/cagatayogdu/Image-classification-with-Gradcam/assets/160175656/8da2b351-c864-4bb9-b0d2-5ed681aad9db)

Above, the Pipeline Schema of the proposed pretrained model is provided.

## Experimental Results

Below is the heatmap of a cultural heritage structure created using the EfficientNetB7 model. In this heatmap, it is determined that the structure is 89.36% damaged based on the prediction.

![image](https://github.com/cagatayogdu/Image-classification-with-Gradcam/assets/160175656/e4c22141-01b3-4c88-b0a2-6901ba238e37)

The following image shows the heatmap of a cultural heritage structure based on the prediction using the Xception model, indicating that the structure is 92.25% damaged. In the heatmap, areas in red indicate more damage. This demonstrates the effectiveness of the model in detecting damage.

![image](https://github.com/cagatayogdu/Image-classification-with-Gradcam/assets/160175656/8a8ab262-835e-41d8-885a-fcb885bd489b)

