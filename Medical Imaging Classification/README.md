Description:

This project involves building a deep learning pipeline to classify medical images, drawing from real-world data and deploying robust models. The project highlights the ability to preprocess data, implement and compare multiple models (including transfer learning), and interpret model performance. 

Models used include CNNs with a variety of fine-tuning applied to pooling and layers. Models with specific applications to classification such as ResNet, AlexNet, and Inception V3. 

The results of these models were compared with each other using test accuracy scores as well as epochs and batch sizes. 

A variety of data engineering techniques are also employed to improve the accuracy of the models. A primary method is synthetic data generation through augmentation 

It appears that Inception V3 performed the best out of our 3 models (Improved CNN, AlexNet, and Inception V3), achieving test accuracy of 88%. The CNN and AlexNet has a simplistic, shallow architecture and may not be able to capture complex patterns in medical images. Even with augmentation, the CNN model had fewer parameters to learn the subtle variations. This is evident in the erratic training curves for both CNN and AlexNet, compared to the smoother curve for Inception V3.

Out of all the models, ResNet50 with fine-tuning performed the best, achieving test accuracy of 95.58%. Through residual learning and fine-tuning, the model was able to adapat its pre-trained weights to medical images.

From this classification exercise, we can provide insights on how we can apply ML techniques specific to each domain. Further study using this dataset would be able to to aid healthcare professionals in interpretting radiology reports and provide diagnostic support.



