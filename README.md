## TASK

Our objective is to develop a machine learning model capable of classifying 555 bird species and compete in [the Kaggle Competition](https://www.kaggle.com/competitions/birds23wi "Birds Birds Birds Are they real?")

## Data Set

We have been provided with a dataset comprising 38,561 images of 555 distinct bird species to train our machine learning algorithm. Additionally, a separate subset of 10,000 images has been designated for testing without labels.

#### Some Sample Images
![0aab634961514bd5b30ecdec7f07257d](https://user-images.githubusercontent.com/45305014/224658729-dc8676a9-f325-4599-9b6f-5cfe093d6b55.jpg)
![0acd9c0bfbdc4de980da093bd3bac43c](https://user-images.githubusercontent.com/45305014/224658734-a3feaf97-3965-40d8-8fd5-a8ff0bdd92cc.jpg)
![0adb3cc233a44d15a05c811d0b289587](https://user-images.githubusercontent.com/45305014/224658737-c3c6bbb9-f09b-42ee-b0f2-7bd279ff43bf.jpg)
![0adc0bc36fca4078be6fd45ddf1653d5](https://user-images.githubusercontent.com/45305014/224658739-87097b5b-2b08-4b10-92af-350a6ca60523.jpg)


## Preprocessing and Augmentation

We conducted a series of tests to evaluate the impact of different combinations of image transformations on the performance of the RESNET 18 model. These transformations included random cropping, flipping, rotation, Gaussian noise, color inversion, and color jitter. We aslo performed batch normalization. Our testing approach was identical to that used in [Tutorial 4 - Transfer Learning to Birds.ipynb.](https://colab.research.google.com/drive/1kHo8VT-onDxbtS3FM77VImG35h_K_Lav?usp=sharing). We used 20 percent of training data to measure the effects of the transforms. We didn't see significant accuracy increase with any of the transforms in first 10 epochs or so. We think the reason for that the features that differentiates the bird species are sometimes very suttle 

