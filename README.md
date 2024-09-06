# CSST106-CS4B-MP1
 Exploring the Role of Computer Vision and Image Processing in AI

https://github.com/user-attachments/assets/08604719-b9f6-4f53-b181-7c3a0a190299

# **Introduction to Computer Vision and Image-Processing**

**Computer Vision (CV)**

Computer Vision (CV) is a field of AI that enables computers to interpret and understand images and videos. It allows machines to recognize objects, people, and patterns, simulating human visual abilities. CV is essential for applications like facial recognition, object detection, and autonomous driving.

**Image Processing**

Image Processing is the first step in preparing visual data for CV. It involves converting images into a digital format and applying techniques to improve their quality, enhance features, and extract useful information. This step is crucial for ensuring that the images fed into CV systems are clear and informative.

**Importance for AI Systems**

For AI systems to function effectively, they must handle and analyze images accurately. Image processing helps by enhancing and cleaning up visual data, which allows CV models to recognize patterns and make precise decisions. Proper image processing ensures that AI systems can interpret visual information correctly and perform tasks reliably.


# **Types of Image Processing Techniques**

Image processing involves enhancing and manipulating images to achieve various results. It can improve image quality, remove unwanted objects, or even create entirely new images. For example, image processing can be used to remove the background from a photo, leaving only the main subject.

This field includes a range of techniques and algorithms designed to perform different tasks. This section will cover some common image processing tasks and how they are performed.

**1. Image Restoration**

Images can degrade over time, especially older ones from before cloud storage was common. For example, photos from old instant cameras may get scratched. Image Restoration is an important technique used to fix these damaged images. Advanced methods, including Deep Learning, can help recover missing parts of old or torn documents, revealing information that was lost.

The example below shows an old photo that, with the help of image restoration, has been restored to its original appearance.

![Screenshot 2024-09-06 at 11 02 30](https://github.com/user-attachments/assets/898153e7-fb26-4f01-90a2-0e521b37555a)
_Figure 1. Image Restoration_

**2. Object Detection**

Object Detection involves finding and identifying objects in an image. It’s commonly used in security and surveillance. The most common method uses Deep Learning, especially Convolutional Neural Networks (CNNs), to detect objects accurately.

The example below shows how object detection is used in highway security cameras to identify and monitor vehicles.

![Screenshot 2024-09-06 at 11 03 13](https://github.com/user-attachments/assets/f6462662-56f6-42c0-9c92-fea981f420b3)
_Figure 2. Object Detection_

**3. Image-to-Image Translation**

Image-to-Image Translation involves learning how to transform one type of image into another. For example, you can input a free-hand sketch and get a realistic image of the object from that sketch. This is done by training a model with pairs of related images as shown below.

![Screenshot 2024-09-06 at 11 03 37](https://github.com/user-attachments/assets/758d87e1-70b7-4136-b631-8d5b00073ca7)
_Figure 3. Image-to-Image Translation_


# **Case Study**

This case study explores a real-world AI application that uses computer vision specifically **object detection in** **Sports Analytics**. It focuses on a data-centric approach to analyzing and interpreting sports data through computer vision techniques.

**Sports analytics** uses computer vision to analyze sports videos and extract important insights. By applying techniques like object detection and tracking, computer vision models can identify and follow players, balls, and other objects during a game. This allows for automatic data collection on player positions, ball movements, pass accuracy, shot speed, and more. These insights help teams understand strategies, player performance, and game dynamics.

https://github.com/user-attachments/assets/5a0a776b-c1c9-4e5f-9225-b30d1f577082

However, this application faces challenges like data imbalance and label quality. For example, detecting and tracking the ball in a football match can be difficult due to its small size and fast movement. A **data-centric approach** improves model performance by ensuring the training data is high-quality, balanced, and accurately labeled, enabling the model to better recognize all objects and accurately analyze game footage.


# **Image Processing Implementation** 

**Player Detection and Tracking in Soccer Matches**

Based on the case study I chose, which is **object detection**, I believe it will greatly help sports analytics. To support this, I have an image-processing implementation for **Player Detection and Tracking in Soccer Matches**. In sports analytics, accurately detecting and tracking players on the field during a soccer match is crucial for analyzing team formations, player movements, and tactical strategies. A simple yet effective problem to tackle is "Detecting and tracking all players on the field in a soccer match video."

To address this problem, we can create an image processing model that combines image segmentation with object detection algorithms. This model will detect each player and track their movements across video frames.


**1. Preprocessing:**

Convert each frame of the video to grayscale to simplify the data, reducing computational load and improving processing speed.
Apply Gaussian Blur to reduce noise and smoothen the image, helping the model focus on relevant features.

**2. Image Segmentation:**

Use a Background Subtraction technique to separate the moving players (foreground) from the static background (field). This technique is effective in highlighting players by subtracting the static field background from each frame.

**3. Object Detection:**

Apply a Bounding Box Detection method using algorithms like YOLO (You Only Look Once) or SSD (Single Shot MultiBox Detector) to detect each player as an object within each frame. Bounding boxes will be drawn around detected players to isolate them from the background.

**4. Object Tracking:**

Implement a Multi-Object Tracking algorithm (like SORT - Simple Online and Realtime Tracking) to track each detected player across multiple frames. The algorithm will assign a unique ID to each player and follow them as they move around the field.

**5. Post-Processing and Analysis:**

Use the tracked player positions to analyze player movements, formations, and tactical strategies. The data can help in understanding player positioning, stamina, and team coordination.

**Effectiveness of the Model:** This model is effective in solving the problem of player detection and tracking by using a combination of background subtraction, object detection, and multi-object tracking techniques. It provides a foundation for advanced sports analytics, enabling automated analysis of player performance and game tactics.


# **Conclusion**

Effective image processing is key to making AI systems work well, especially in areas like sports analytics where accurately finding and tracking players and the ball is important for understanding the game. By processing images correctly, separating important parts, and using detection and tracking methods, AI can gather useful insights for better decision-making. This activity taught me how different image processing techniques must be combined to solve specific problems and how these steps help AI models perform better and provide more reliable analysis.

![Screenshot 2024-09-06 at 15 20 46](https://github.com/user-attachments/assets/c4b1caf0-1d00-45eb-aa26-802218879802)

# **References**

 - Bose, B. (2022, April 27). Introduction to Basic Computer Vision & Image Processing. Medium; Medium. https://bishalbose294.medium.com/introduction-to-basic-computer-vision-image-processing-f692aa1a4f18

- Rouse, M. (2019). Techopedia - Where Information Technology and Business Meet. Techopedia.com. https://www.techopedia.com/

- Image Processing: Techniques, Types, & Applications [2023]. (n.d.). Www.v7labs.com. https://www.v7labs.com/blog/image-processing-guide#image-processing-techniques

- The Tenyks Blogger. (2023, November 8). Sports Analytics — A Data-Centric Approach to Computer Vision. Medium; Medium. https://medium.com/@tenyks_blogger/sports-analytics-a-data-centric-approach-to-computer-vision-246f19cf8a04

- Boesch, G. (2023, November 28). Computer Vision Trends - The Ultimate 2024 Overview - viso.ai. Viso.ai. https://viso.ai/computer-vision/computer-vision-trends/#:~:text=Edge%20Computing%20and%20Lightweight%20Architecture

















































