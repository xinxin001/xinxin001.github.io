# Artistic Animals Blog #

## 5 December 2020 ##
I've deployed the model on a simple Flask and React app, and you can access its predictions [here](https://xinxin001.github.io/ArtisticAnimalsWebApp/)

## 4 December 2020 ## 
![train](/images/gan/final_output_sample.png)
Final implementation of the model used Spectral Normalization and Convolutional Neural Networks for both the Discriminator and the Generator. I've been mostly dealing with problems managing the resources on Google Colab and Kaggle(exceeding RAM usage, training time, etc...). I've since scaled down on the resolution. After multiple trainings averaging at 12hrs each. The results displayed have been the best I've got.

## 7 November 2020 ##
![train](/images/gan/train-129.png)
I am going to try implementing a DCGGAN, as it seems the regular GAN is too unstable, DCGAN is said to be more stable and be able to generate higher quality images, and it can be used for style transfer, which fits my broader goals. However, the results are not very convincing either. I think I need to focus more on hyperparameter tuning.

## 3 November 2020 ##
I automated more of my GAN training process. Before it was really hacky where I had to run individual code blocks, restart runtime, do something, then run another codeblock, and often not in order. Now I can just press 'Run All', and there is a smooth pipeline from Imports->Data Preprocessing->Defining Model->Training->Saving Results

## 30 October 2020 ## 
![dogs](/images/gan/dogs.png)
![cdog](/images/gan/cdog.png)
After getting further studying my dataset. I realized that bounding boxes were provided along with the dataset, that could focus on more on invididual dogs instead of the noise around it. I've coded a preprocessing method that extracts the contents of each bounding box, and as a result should be much easier for the model to handle.

## 25 October 2020 ## 
![sample](/images/train-50.png)
![loss](/images/loss_history.png)
I've set up my notebook and worked on the data processing part. I am using the Stanford Dog dataset, which contains 120 different breeds of dogs, and around ~170 pictures for each dog. I moved all the pictures in one big folder for easier manipulation with code. And fed them data into the basic GAN as described in the **Generative Deep Learning** book. It gave really poor results, and the Discriminator/Generator loss plateau-ed really fast, with little convergence. At this moment, I am only focusing on generating pictures of dogs, I will leave the style transfer on hold for now.

## 20 October 2020 ## 
I'm going to use **Generative Deep Learning, by David Foster** as reference for my project. 
