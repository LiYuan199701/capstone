# capstone
This repo is to store and track my capstone project progress, including files, results, codes, and plots.

I use a prefix number to indicate the order of the code file and suffix name to indicate the functionality of a file.



# Automatically label medical benchmark images without human manually operation

Nowadays, in hospitals and medical or healthcare system, millions images are generated for patients, treatments and research. However, most of them are unlabelled. To do downstream analysis, labelled images are imperative, but human manually labeling images consumes a large amount of time, thus it is impossible to do that. However, as convolution neural network and natural langauge processing develop, humans are able to label images by taking use of these start-of-the-art techniques automatically without handcarfting.

In order to test my idea and method, I have to find a benchmark medical image database which is light and standard, making the test easier to go on.

## The benchmark image dataset – MedMNIST v2

> We introduce MedMNIST v2, a large-scale MNIST-like collection of standardized biomedical images, including 12 datasets for 2D and 6 datasets for 3D. All images are pre-processed into 28x28 (2D) or 28x28x28 (3D) with the corresponding classification labels, so that no background knowledge is required for users. Covering primary data modalities in biomedical images, MedMNIST v2 is designed to perform classification on lightweight 2D and 3D images with various data scales (from 100 to 100,000) and diverse tasks (binary/multi-class, ordinal regression and multi-label). The resulting dataset, consisting of 708,069 2D images and 10,214 3D images in total, could support numerous research / educational purposes in biomedical image analysis, computer vision and machine learning. We benchmark several baseline methods on MedMNIST v2, including 2D / 3D neural networks and open-source / commercial AutoML tools.

![MedMNISTv2_overview](img/medmnistv2.jpg)

For more information on this dataset, please refer to (https://github.com/LiYuan199701/MedMNIST)
