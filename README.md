# face-detection-blur
This notebook presents a computer vision method Using haar cascade classifier for face detection and gaussian blur, I got this output of detecting 12 faces and blurring them, this can be applied in instances where identity privacy is crucial, and in the scope of Biomedical Engineering, it can be applied to anonymize patient identity:
 
 <p align="center">
<img width="512" height="389" alt="__results___6_0" src="https://github.com/user-attachments/assets/48157f55-066b-4cff-9c45-8453e8c3ed5c" />


# Dataset
data is from kaggle: [face detection dataset](https://www.kaggle.com/datasets/iamtushara/face-detection-dataset/data)

# Workflow

we need to convert BGR images to gray, bacause face detection works more efficiently in grayscale.
 <p align="center">
<img width="512" height="389" alt="__results___3_0" src="https://github.com/user-attachments/assets/ac0e3c6c-2dab-49d3-b1d2-30629f064fd0" />
  
Then, we apply cv2.CascadeClassifier to specifiy region of pretrained model we want to detect, in this case I wanted to detect the faces so I did haarcascade_frontalface_default.xml.

