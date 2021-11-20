# CoviDetector: COVID-19 Detection Using Chest X-Ray Images
COVID-19 has become a serious health problem all around the world. It is confirmed that this virus has taken over 51,40,000 lives until today. Since the beginning of its spreading, many researchers developed systems and methods for predicting the virus's behavior or detecting the infection. One of the possible ways of determining the patient infection to COVID-19 is through analyzing the chest X-ray images. As there are a large number of patients in hospitals, it would be time-consuming and difficult to examine lots of X-ray images, so it can be very useful to develop a system that does this job automatically.

In this project, I have built a CNN Model that detects the COVID-19 infection in the patient which is trained on approx. 300 Chest X-Ray images belonging to two categories: Covid Infected and Normal.

The input is given in the form of a Chest X-Ray image and the output tries to predicts whether the patient is infected with the COVID-19 virus or not by classifying the image into one of the following two categories:
1. Covid Infected
2. Normal

The dataset of images used in this project, containing images of Chest X-Ray images, can be viewed [here](https://www.kaggle.com/fusicfenta/chest-xray-for-covid19-detection). In the proposed CNN Architecture, there are four convolution layers with 32 filters in the first layer, 64 filters in the second and third layer and 128 filters in the last layer. The training accuracy is obtained to be 86%.

### Mobile Android Application
[Click here]() to watch the video.

### Web Application
[Click here](https://covidetector-chest-xray.herokuapp.com/) to go to the website.

### CNN Model Architecture
![CNN Model](https://i.ibb.co/6XFYXkT/CNN-Architecture.png "CNN Model")

### Python Notebook
The .ipynb notebook can be accessed [here](https://nbviewer.org/github/lakkshh/CoviDetector-Covid-19-Detection/blob/master/training.ipynb).

### Novelty
Various Covid-19 detection systems exist that detect the presence of Covid-19 virus using Chest X-Ray images with the help of Transfer Learning by using networks like ResNet50V2, Xception network etc. I have tried to build the same system with a relatively simpler architecture using a CNN model created from scratch. It is observed that the results obtained are quite good and can further improve if trained with an even larger dataset.

- Built the CNN Model from scratch and Hyper-Parameter Tuning
    - Built the CNN model from scratch using trial and error for the number of convolution layers, dropout and max-pool layers, filter size, epochs etc. thus, achieving a train accuracy of 86%..
- Optimizations
    - Built a tensorflow input pipeline and created equal sized 32 batches to handle the large dataset and optimize performance
    - Used concepts of caching, shuffling and prefetching to optimize the tensorflow input pipeline performance while handling the large dataset
    - Applied Data Augmentation to generate new training examples from existing training set using transformations like Flipping and Rotation to prevent overfitting and increase robustibility
    - Added links to book vaccination slot, if person is healthy and nearest hospital, if infected, on the portal itself

### Methodology Flow Chart
![Methodology](https://i.ibb.co/YBHXSQ4/Methodology.jpg "Methodology")

### I/O Screenshots (Web App)
- Home Page Layout
![Layout 1](https://i.ibb.co/8MPhwgK/1-Home-Page-Layout-1.png "Layput 1")
![Layout 2](https://i.ibb.co/mh7rnX2/2-Home-Page-Layout-2.png "Layput 2")

- Upload Image
![Upload Image](https://i.ibb.co/1djgWSV/3-Upload-Image.png "Upload Image")

- Prediction
![Prediction 1](https://i.ibb.co/xgWR9vX/4-Prediction-1.png "Prediction 1")
![Prediction 2](https://i.ibb.co/bg1vzxb/5-Prediction-2.png "Prediction 2")

### I/O Screenshots (Android App)
- Home Page Layout
<img src="https://i.ibb.co/Yy8tQp8/1-Mobile-Layout-1.jpg" height="800">
<img src="https://i.ibb.co/f9hNH5d/2-Mobile-Layout-2.jpg" height="800">

- Upload Image
<img src="https://i.ibb.co/QFqYLbm/3-Mobile-Upload-Image.jpg" height="800">

- Prediction
<img src="https://i.ibb.co/JC4wkQb/4-Prediction-1.jpg" height="800">
