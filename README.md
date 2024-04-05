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

![Screenshot 2024-04-03 225747](https://github.com/KHADAR134/Projectwork2/assets/75235233/d28fbf1d-f945-44d3-9369-2a77e8e17d31)


## Output

#### Output1 - Detection For Image

![image](https://github.com/KHADAR134/Projectwork2/assets/75235233/f6a51735-dff4-4c2f-8b1a-9548ba1c4a09)


#### Output2 - Detection For Video

![image](https://github.com/KHADAR134/Projectwork2/assets/75235233/46075a7c-9217-4fa5-ac53-7045300fe73d)



## Results and Impact
1)Implementing a YOLO-based weapon detection system in live streams and videos enhances security by swiftly identifying weapons.

2)Email notifications promptly alert authorities, enabling rapid response to potential threats.

3)Users experience heightened safety and peace of mind in public spaces and sensitive environments.

4)Real-time monitoring fosters proactive measures against violence and unlawful activities.

5)The system minimizes human error and improves overall surveillance efficacy.

6)It empowers law enforcement to intervene swiftly, preventing potential harm.

7)Public trust in safety measures is bolstered, fostering a sense of security and wellbeing.

8)Ultimately, the integration of YOLO technology enhances situational awareness and promotes safer communities.

## Articles published / References
[1] P. Mohanty, A. Tushir, and A. Patwardhan, "Weapon detection in surveillance videos using YOLO v3," in 2019 3rd International Conference on Computing Methodologies and Communication (ICCMC), 2019, pp. 1204-1208.Link: https://ieeexplore.ieee.org/document/8930745

[2]  S. E. Elmahmoud, A. E. Hassanien, and A. S. Elmahallawy, "Firearm detection in videos using deep learning," in 2019 IEEE International Conference on Systems, Man and Cybernetics (SMC), 2019, pp. 3854-3859.Link: https://ieeexplore.ieee.org/document/8914411

[3]  S. Al-Din, M. F. Fazal, and M. Arif, "Firearm detection in videos using deep learning," in 2020 8th IEEE International Conference on Engineering Technologies and Applied Sciences (ICETAS), 2020, pp. 1-6.Link: https://ieeexplore.ieee.org/document/9333619

[4]  H. Yuan, H. Xia, J. Wu, Z. Wang, and Z. Yang, "Firearm detection in surveillance videos based on YOLOv3," in 2021 4th International Conference on Mechatronics, Control and Robotics (ICMCR), 2021, pp. 242-246.Link: https://ieeexplore.ieee.org/document/9392905

[5]  A. Khokhar, M. A. Khan, M. Arif, and S. Iqbal, "Firearm detection in surveillance videos using deep learning," in 2020 IEEE International Conference on Consumer Electronics - Taiwan (ICCE-TW), 2020, pp. 1-4.Link: https://ieeexplore.ieee.org/document/9259631

[6]  S. O. Vimal, R. Rekha, and S. S. Vinay, "Gun detection using deep learning techniques," in 2021 4th International Conference on Intelligent Sustainable Systems (ICISS), 2021, pp. 2295-2300.Link: https://ieeexplore.ieee.org/document/9436266

[7]  V. Agarwal, S. M. Ak, R. Kumari, and P. Tripathi, "Firearm detection in video surveillance using deep learning techniques," in 2020 3rd International Conference on Computing, Communication and Security (ICCCS), 2020, pp. 1-6.Link: https://ieeexplore.ieee.org/document/9189023

[8]  X. Zheng, J. Zhang, and L. Zhu, "Firearm detection based on improved YOLOv3," in 2021 IEEE International Conference on Artificial Intelligence and Virtual Reality (AIVR), 2021, pp. 284-289.Link: https://ieeexplore.ie







