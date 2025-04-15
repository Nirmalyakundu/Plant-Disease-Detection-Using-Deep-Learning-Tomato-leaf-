Plant Disease Detection Using Deep Learning (Tomato Leaf)

This project focuses on developing an advanced deep learning system to detect tomato leaf diseases, aiming to assist farmers in early diagnosis and intervention. Traditional methods like expert inspection are often time-consuming and error-prone. Leveraging machine learning, particularly deep learning, allows for efficient, accurate, and automated disease identification.

The team used a dataset of 23,000 labeled RGB images representing ten categories of healthy and diseased tomato leaves. The dataset was split into 85% training, 15% validation, and a small portion for testing. Image preprocessing steps like resizing (to 128×128), normalization (pixel values scaled between 0 and 1), and data augmentation were applied to enhance model performance and generalization.

EfficientNetB0, a pre-trained convolutional neural network (CNN), served as the model’s foundation. The architecture excluded its top layers to add custom ones tailored to the classification task. These included Global Average Pooling, Dropout layers (rate = 0.5), and Dense layers with ReLU and softmax activations for multi-class output. The model was compiled using the Adam optimizer (learning rate = 1e-5), Categorical Crossentropy loss, and accuracy as the evaluation metric.

Challenges like variable image quality and class imbalance were tackled with normalization and targeted data augmentation. After training for 20 epochs, the model achieved a remarkable 99.91% training accuracy and 99.04% validation accuracy.

Looking ahead, the project aims to scale the model for other crops like rice and wheat, and to integrate it into real-time applications such as mobile or web apps. This would enable farmers to upload leaf images and instantly receive a disease diagnosis, revolutionizing agricultural practices through accessible AI technology.

Our team consists of four passionate members: Ashutosh Rana, Jaydev Jana, Nirmalya Kundu, and Ipsita Sahoo. Under the guidance of our mentor, Amlan Roy Chowdhury, we worked collaboratively on every aspect of the project. From data preprocessing to building and fine-tuning the deep learning model, each of us brought unique strengths to create a powerful tool for plant disease detection.
