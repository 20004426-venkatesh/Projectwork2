## Harnessing Deep Learning for Fabric Defect Detection
Fabric defect detection is a quality control process that has to ensure the identiﬁcation of defects present in the textile fabric. . A traditional inspection system is composed of manual workers/operators. Their job is to detect the defects while the fabric is being moved by a machine. Traditionally, this motorized machines unroll the fabric rolls, so that the fabric is stretched and presented to the worker without folds and thickness differences. As this process relies on human visual ability and concentration, this task can be very tedious and time-consuming, which can lead to fatigue and consequently human error. Therefore, traditional systems can only achieve a 40% to 50% accuracy, even though they have very slow speed compared to production rate. As a result, automatic visual inspection systems to ensure the high quality of products in production lines are in increasing demand. In order to reduce these costs, a fast and automatic defect detection system, which can be complemented with the operator . To perform the task of defect detection, a custom Convolutional Neural Network (CNN) was used.
## About
The CNN architecture was created from scratch, with Convolutional, Max-pooling, ReLU and Dense layers. No pre-trained networks or weights were used. In order to obtain the best architecture/conﬁguration various training and tests were performed with the chosen datasets. The selected datasets were collected from various sources, in order to compare and test this model against existing works. Layer feature visualization and exhaustive testing on four different datasets, also constitute contributions that are not usually seen in similar works. The proposed system presents high accuracy and lower execution time, in comparison with related works. The interaction between the system and the operator, complemented by the use of FN reduction methods, constitutes a novel approach to this problem.

Although the mentioned methods may present high ac-curacy rates in defect detection, some are computationally inefﬁcient. Moreover, their accuracy may not be very high when many fabric defect types are considered. It is important to note that these methods were used with different purposes (defect detection, defect segmentation, and defect classiﬁcation); however, in this work we are just focused on defect detection.

## Features
The project you described involves several components and features. Here's a breakdown of the main features of the Harnessing Deep Learning for Fabric Defect Detection:

1.**Data Collection and Preparation**:

Gather a large dataset of fabric images containing both defective and non-defective samples. These images should cover various types of defects, lighting conditions, and fabric textures.
Annotate the images to provide ground truth labels indicating the presence and location of defects.

2.**Preprocessing**:

Resize the images to a consistent resolution to ensure uniformity across the dataset.
Normalize pixel values to a common scale (e.g., [0, 1] or [-1, 1]) to improve model training convergence.
Augment the training dataset with transformations such as rotation, flipping, and scaling to increase its diversity and robustness.

3.**Model Selection**:

Choose an appropriate deep learning architecture for fabric defect detection. Convolutional Neural Networks (CNNs) are commonly used due to their effectiveness in image-related tasks.
Consider architectures such as Faster R-CNN, YOLO (You Only Look Once), or SSD (Single Shot Multibox Detector) which are well-suited for object detection tasks

4.**Model Training**:

Initialize the selected model with pre-trained weights on a large-scale image dataset (e.g., ImageNet) to leverage feature representations learned from general images.
Fine-tune the model on the fabric defect dataset using transfer learning techniques. Train the model to predict both the presence and location of defects within the fabric images.
Utilize techniques like stochastic gradient descent (SGD) with adaptive learning rate schedulers and regularization methods (e.g., dropout) to prevent overfitting.

5.**Model Evaluation**:

Assess the performance of the trained model on the validation set using metrics such as mean Average Precision (mAP), Precision-Recall curves, and Intersection over Union (IoU).
Fine-tune hyperparameters based on validation performance to optimize the model's generalization ability.

6.**Model Testing and Deployment**:

Evaluate the final model on the held-out testing set to obtain unbiased performance estimates.
Integrate the trained model into the fabric inspection pipeline or system for real-time or batch defect detection.
Implement mechanisms for model monitoring, versioning, and retraining to maintain performance as new data becomes available







## Requirements
1. Operating System: Compatible with Windows, macOS, and Linux distributions.
2. Programming Language: Utilize Python for backend development.
3. Framework: Implement YOLO (You Only Look Once) pre-trained model for real-time object detection.
4. Integration: Incorporate OpenCV library for image and video processing.
5. Email Notification: Integrate SMTP protocol for sending email notifications upon detection.
6. Database: Implement SQLite for storing detection records and configuration settings.
7. User Interface: Develop a user-friendly interface using libraries such as Tkinter or PyQt.
8. Logging: Utilize logging module for recording system activities and errors.
9. Deployment: Package the application into executable files for easy deployment.
10. Documentation: Provide comprehensive documentation including installation guide, usage instructions, and troubleshooting tips..

## System Architecture


![image](https://github.com/20004426-venkatesh/Projectwork2/assets/75234983/91732d92-696a-4d75-b00d-a74fac8a781c)



## Output

#### Output1 - Detection For fabric detection

![image](https://github.com/20004426-venkatesh/Projectwork2/assets/75234983/5915ae20-9b19-4d1b-9a8d-726b4fa90662)

![image](https://github.com/20004426-venkatesh/Projectwork2/assets/75234983/6270dcb2-92b9-40a9-bdde-b1021167d20b)










## Results and Impact
Fabric defect detection plays an increasingly important role in the industrial automation application for fabric production, but how to detect defects rapidly and accurately is still challenging. In this study, we propose a powerful fabric defect detection method using a hybrid of convolutional neural network (CNN) and variational autoencoder (VAE). The convolutional layers are used for extracting fabric image pattern features and the variational autoencoder is used for modeling the latent characteristics and inferring a reconstruction. The defect positions can be detected by the differences between the original image and the reconstruction image. The proposed method is validated on public patterned fabric datasets. The experimental results demonstrate that the proposed model can achieve outstanding performance in both image level and pixel level defect detectionwha

## Articles published / References
•	Y. F. Zhang and R. R. Bresee , “Fabric Defect Detection and Classiﬁcation Using Image Analysis,” Text. Res. J., vol. 65, pp. 1–9, 1995, doi:10.1177/004051759506500101
•	A. Ghosh, “Pattern classiﬁcation of fabric defects using support vector machines,” Int. J. Cloth. Sci. Technol., vol. 23, pp. 142–151, 2011, doi:10.1108/09556221111107333.
•	F. Tajeripour ,E. Kabir, and A. Sheikhi , “Fabric defect detection using modiﬁed local binary patterns,” EURASIP J. Adv. Signal Process., vol.2008, 2008, doi: 10.1155/2008/783898
•	C. Kwak, J. A. Ventura, and K. Tofang-Sazi, “Automated defect inspection and classiﬁcation of leather fabric,” Intell. Data Anal., no. May, pp.355–370, 2001, doi: 10.3233/IDA-2001-5406.
•	K. L. Mak, P. Peng, and K. F. C. Yiu, “Fabric defect detection using morphological ﬁlters,” Image Vis. Comput., vol. 27, no. 10, pp. 1585–1592,2009, doi: 10.1016/j.imavis.2009.03.007
•	A. Conci and C. B. Proença, “A fractal image analysis system for fabric inspection based on a box-counting method,” Comput. Netw. ISDN Syst,vol. 30, no. 20, pp. 1887–1895
•	L. M. Hoffer, F. Francini, B. Tiribilli, and G. Longobardi, “Neural net-works for the optical recognition of defects in cloth,” Opt. Eng., pp.3183–3190, 1996, doi: 10.1117/1.601057
•	D. Tsai and C. Hsieh, “Automated surface inspection for directional textures,” Image Vis. Comput, vol. 18, no. 1, pp. 49–62, 1999
•	A. C. Bovik, M. Clark, and W. S. Geisler, “Multichannel Texture Analysis Using Localized Spatial Filters,” IEEE Trans. Pattern Anal. Mach. Intell.,vol. 12, no. I, pp. 55–73, 1990B. N. Nickolay and H. 
  Schmalfub, "Automatic fabric inspection – utopiaor reality?," Mellind Textilberichte, vol. 73, pp. 33-37. 1993 
•	A. Kumar, “Computer-Vision-Based Fabric Defect Detection: A Survey,”IEEE Transactions on Industrial Electronics, vol. 55, no. 1, pp. 348–363,2008







