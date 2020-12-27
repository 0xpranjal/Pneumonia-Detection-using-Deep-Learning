# Pneumonia Detection using Deep Learning

## Problem Statement

**Build a binary classifier to detect pneumonia using chest x-rays.**

### Pneumonia
> Pneumonia is an infection that inflames the air sacs in one or both lungs. The air sacs may fill with fluid or pus (purulent material), causing cough with phlegm or pus, fever, chills, and difficulty breathing. A variety of organisms, including bacteria, viruses and fungi, can cause pneumonia.  Chest X-ray, blood tests, and culture of the sputum may help confirm the diagnosis. The disease may be classified by where it was acquired, such as community- or hospital-acquired or healthcare-associated pneumonia.

## Dataset description

> The dataset is organized into 3 folders (train, test, val) and contains subfolders for each image category (Pneumonia/Normal). There are 5,863 X-Ray images (JPEG) and 2 categories (Pneumonia/Normal).
Chest X-ray images (anterior-posterior) were selected from retrospective cohorts of pediatric patients of one to five years old from Guangzhou Women and Children’s Medical Center, Guangzhou. All chest X-ray imaging was performed as part of patients’ routine clinical care. For the analysis of chest x-ray images, all chest radiographs were initially screened for quality control by removing all low quality or unreadable scans. The diagnoses for the images were then graded by two expert physicians before being cleared for training the AI system. In order to account for any grading errors, the evaluation set was also checked by a third expert.

<p align="center"><img height="350" width="700" src="Assests/pneumonia_train.png"  ></p>

## Model used :
**Here is a small comparison of all the models tested in the project:**

<p align="center"><img height="350" width="700" src="Assests/comparison.png"></p>

- ### Convolutional Neural Network

<p align="center"><img height="350" width="700" src="Assests/cnn.png"></p>

```
624/624 [==============================] - 11s 18ms/step
Loss of the model is -  0.30433156475042683
624/624 [==============================] - 10s 15ms/step
Accuracy of the model is -  91.98718070983887 %
```
<p align="center"><img height="350" width="700" src="Assests/model_accuracy.png"></p>

- ### Convolutional Neural Network(Different approach) :

<p align="center"><img height="350" width="700" src="Assests/accuracy_cnn_2.png"></p>

```
624/624 [==============================] - 30s 49ms/step
Test Accuracy: 68.91%
652/652 [==============================] - 338s 518ms/step
Train Accuracy: 66.33%
```

- ### DenseNet :

<p align="center"><img height="350" width="700" src="Assests/densenet.png"></p>

<p align="center"><img height="350" width="700" src="Assests/densenetperf.png"></p>

```
624/624 [==============================] - 132s 211ms/step
Test Accuracy: 87.18%
652/652 [==============================] - 622s 954ms/step
Train Accuracy: 86.22%
```
- ### VGG16 :

<p align="center"><img height="350" width="700" src="Assests/vgg16.png"></p>

<p align="center"><img height="350" width="700" src="Assests/vgg16_perf.png"></p>

```
624/624 [==============================] - 226s 363ms/step
Test Accuracy: 66.19%
652/652 [==============================] - 1608s 2s/step
Train Accuracy: 82.63%
```


- ### ResNet :

<p align="center"><img height="350" width="700" src="Assests/resnet.png"></p>

```
624/624 [==============================] - 101s 162ms/step
Test Accuracy: 73.40%
652/652 [==============================] - 651s 999ms/step
Train Accuracy: 88.92%
```

- ### InceptionNet :
<p align="center"><img height="350" width="700" src="Assests/inceptionnet.png"></p>

```
624/624 [==============================] - 41s 66ms/step
Test Accuracy: 76.76%
652/652 [==============================] - 295s 453ms/step
Train Accuracy: 91.26%
```
