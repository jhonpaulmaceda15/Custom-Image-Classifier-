### Custom-Image-Classifier- 
## https://colab.research.google.com/drive/1Fi642Dr700o57v0pg-xkZmJTRiu__VvF?usp=sharing
## A. Project Overview

This project focuses on developing an image classification system that can identify different plant species using machine learning techniques. The system is trained on a dataset containing multiple plant images and uses a deep learning model to classify them accurately.

The main purpose of this image classification model is to:

Automatically identify plant species from images
Assist in agriculture, education, and environmental monitoring
Reduce manual effort in plant identification
Provide a foundation for smart farming applications
## B. Plant Species Section

# 1. Aloe Vera
Scientific Name: Aloe barbadensis miller
Description: A succulent plant known for its thick, fleshy leaves containing gel used for skin treatment, burns, and medicinal purposes.
<img width="500" height="600" alt="image" src="https://github.com/user-attachments/assets/644a53b4-05c6-4f60-ad37-c537a9213f2e" />

# 2. Alugbati Leaves
Scientific Name: Basella alba
Description: A climbing leafy vegetable with soft, thick leaves commonly used in soups and known for its high iron content.

# 3. Bay Leaf
Scientific Name: Laurus nobilis
Description: An aromatic leaf used in cooking to enhance flavor, commonly added to soups and stews.

# 4. Bitter Melon
Scientific Name: Momordica charantia
Description: A tropical vine known for its bitter fruit, often used in cooking and for managing blood sugar levels.

# 5. Chili Leaves
Scientific Name: Capsicum frutescens
Description: Leaves of the chili plant, used in Filipino dishes like tinola; rich in nutrients and mild in flavor.

# 6. Gotu Kola
Scientific Name: Centella asiatica
Description: A small herb known for improving memory and wound healing, often used in traditional medicine.

# 7. Guava
Scientific Name: Psidium guajava
Description: A fruit-bearing plant whose leaves are used medicinally for wounds and digestive issues.

# 8. Kangkong (Water Spinach)
Scientific Name: Ipomoea aquatica
Description: A fast-growing aquatic plant commonly used as a vegetable in stir-fry dishes.

# 9. Lagundi
Scientific Name: Vitex negundo
Description: A medicinal plant used to treat cough, asthma, and respiratory problems.

# 10. Lemon Grass
Scientific Name: Cymbopogon citratus
Description: A fragrant grass used in cooking and herbal medicine, known for its citrus flavor.

# 11. Malunggay Leaves
Scientific Name: Moringa oleifera
Description: A highly nutritious plant rich in vitamins and minerals, often called a “superfood.”

# 12. Mint
Scientific Name: Mentha spp.
Description: An aromatic herb used in food, drinks, and medicine, known for its cooling effect.

# 13. Mugwort
Scientific Name: Artemisia vulgaris
Description: A medicinal herb used for digestion and traditional healing practices.

# 14. Onion
Scientific Name: Allium cepa
Description: A widely used vegetable known for its strong flavor and health benefits.

# 15. Oregano
Scientific Name: Origanum vulgare
Description: A medicinal and culinary herb commonly used to treat cough and colds.

# 16. Pandan
Scientific Name: Pandanus amaryllifolius
Description: A tropical plant with fragrant leaves used in cooking and desserts.

# 17. Periwinkle
Scientific Name: Catharanthus roseus
Description: A flowering plant known for its medicinal properties, especially in cancer treatment research.

# 18. Rice
Scientific Name: Oryza sativa
Description: A staple crop and primary food source for many countries, especially in Asia.

# 19. Sambong
Scientific Name: Blumea balsamifera
Description: A medicinal plant used to treat kidney stones and as a diuretic.

# 20. Tawa-Tawa
Scientific Name: Euphorbia hirta
Description: A herbal plant commonly used in treating dengue and boosting platelet count.

## Provide the configuration used during model training:

Epochs: __________
Batch Size: __________
Learning Rate: __________
Number of Images per Class: __________

(Optional: You may also include model type, e.g., CNN, MobileNet, etc.)

### D. Model Evaluation
## 1. Confusion Matrix

(Insert screenshot here)

Shows how well the model distinguishes between different plant species.
## 2. Accuracy per Class

(Insert screenshot here)

Displays how accurate the model is for each individual plant species.
## 3. Overall Model Accuracy

(Insert screenshot here)

Provides the total accuracy of the model across all classes.



## 1. Dataset Preparation
I organized my dataset in Google Drive by separating images into different folders based on their labels or classes. This makes it easier to manage and access during training. Folder structure is important in TensorFlow because it automatically reads images based on folders, so if it is not organized properly, the model may get wrong or mixed data.

## 2. Model Training
Convolutional layers help the model “see” important features in images like edges, shapes, and patterns, which are useful for classification. We split the data into training and validation sets so the model can learn from one part and be tested on another to check if it is actually learning well and not just memorizing.

## 3. Performance Analysis
The accuracy of my model depends on the training results, and it shows how often the model predicts correctly. The number of images affects performance because more images usually help the model learn better patterns, while too few images can make the model less accurate.

## 4. Critical Thinking
One challenge I encountered was making sure my dataset was clean and balanced because messy or uneven data can affect results. Data augmentation helps improve the model by creating modified versions of images (like flipping or rotating), which gives the model more variety to learn from and improves accuracy.

## 5. Application
A real-world application of my model could be image recognition, like identifying objects, diseases in plants, or sorting items automatically. This system can be integrated into a mobile or web app by connecting the trained model to an API so users can upload images and get instant predictions.

## 1. What signs indicated overfitting in your first model?
In my first model, overfitting was shown when the training accuracy was high but the validation accuracy was much lower. It also felt like the model was doing well on training data but struggling on new or unseen images.

## 2. How did data augmentation affect validation accuracy?
Data augmentation helped improve validation accuracy because it made the dataset more varied. The model learned from different versions of images, so it performed better on new data.

## 3. What is the purpose of dropout layers?
Dropout layers help prevent overfitting by randomly turning off some neurons during training. This forces the model to learn more general patterns instead of memorizing the data.

## 4. Why does data augmentation improve generalization?
Data augmentation improves generalization because it increases the variety of training data. This helps the model handle real-world images better since it has seen different angles, sizes, and variations.

## 5. Compare accuracy before and after improvements.
Before improvements, the model had higher training accuracy but lower validation accuracy. After applying techniques like augmentation and dropout, the validation accuracy improved and became closer to the training accuracy.

## 6. Which technique contributed most to improvement?
Data augmentation contributed the most because it directly improved how the model performs on unseen data by giving it more diverse examples to learn from.

## 7. Why is saving the model important?
Saving the model is important so we don’t need to train it again from scratch. It also allows us to reuse it anytime for predictions or deployment.

## 8. How can this model be deployed in a real-world system?
The model can be deployed by turning it into an API or integrating it into a mobile or web app. Users can upload images, and the system will instantly give predictions based on the trained model.
