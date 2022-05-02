# capstone
This repo is to store and track my capstone project progress, including files, results, codes, and plots.

I use a prefix number to indicate the order of the code file and suffix name to indicate the functionality of a file.

## To reproduce my codes, it is highly recommend that you run all python notebook in the Google Colab rather than local computers. 

If you have to run them on your local computer, please follow up the below instructions and create a new virtual environment for this project and run them in it. **However, it is not gurantee to successfully run all of them due to different package versions and environment settings.**

**Create conda environment on your local system, this is only valid on mac system right now.**

    cd capstone
    conda env create -f environment-mac.yml
    conda activate capstone

# Automatically label medical benchmark images without human manually operation

Nowadays, in hospitals and medical or healthcare system, millions images are generated for patients, treatments and research. However, most of them are unlabelled. To do downstream analysis, labelled images are imperative, but human manually labeling images consumes a large amount of time, thus it is impossible to do that. However, as convolution neural network and natural langauge processing develop, humans are able to label images by taking use of these start-of-the-art techniques automatically without handcarfting.

In order to test my idea and method, I have to find a benchmark medical image database which is light and standard, making the test easier to go on.

## The benchmark image dataset – MedMNIST v2

> We introduce MedMNIST v2, a large-scale MNIST-like collection of standardized biomedical images, including 12 datasets for 2D and 6 datasets for 3D. All images are pre-processed into 28x28 (2D) or 28x28x28 (3D) with the corresponding classification labels, so that no background knowledge is required for users. Covering primary data modalities in biomedical images, MedMNIST v2 is designed to perform classification on lightweight 2D and 3D images with various data scales (from 100 to 100,000) and diverse tasks (binary/multi-class, ordinal regression and multi-label). The resulting dataset, consisting of 708,069 2D images and 10,214 3D images in total, could support numerous research / educational purposes in biomedical image analysis, computer vision and machine learning. We benchmark several baseline methods on MedMNIST v2, including 2D / 3D neural networks and open-source / commercial AutoML tools.

![MedMNISTv2_overview](img/medmnistv2.jpg)

For more information on this dataset, please refer to (https://github.com/LiYuan199701/MedMNIST)

## Read in MedMNIST v2 data with PyTorch

please run the following notebook which is also included in this repo:

[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/drive/13ME07TJxTA6MJHqjSWGwlGN598lUMYFv)

## Apply directly ClIP zero-shot classification models based on ImageNet to this binary classification

please run the following notebook which is also included in this repo:

[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/drive/12wrkG2sgHtYkiBkqLktPYbKxKGf5USOy)

## Train a CNN model on previous output dataset with its predictions and compare results

please run the following notebook which is also included in this repo:

[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/drive/17fD_l1iIU9-4LFRDcgk0iCRfV6EmucbX)

## Run 30 times for generalized tests

please run the following notebook which is also included in this repo:

[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/drive/15tqWswpoKcWnHs2nP0maGy7AuIPDhEj1)
