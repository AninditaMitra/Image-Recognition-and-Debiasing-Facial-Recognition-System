# Image Recognition and Debiasing Facial Recognition System

Facial recognition is essential to our daily lives, like people unlocking their phones, police identifying facial recognition to fight crimes, influencers using social media to create deepfake, and more. This technique is one of the prominent aspects of deep learning to identify faces for various uses. When it comes to practicing this technique for deep learning, we use the CelebA dataset for testing and training models for facial detections, like searching for people with different colors of hair, hats, sunglasses, or even people of gender and race. 

Recent research has highlighted the vulnerabilities of modern machine learning-based systems to bias, especially towards segments of society that are under-represented in training data. Even the seemingly simple task of facial recognition is subject to extreme amounts of algorithmic bias among select demographics. 

In this project we focused on two prominent aspects of applied deep learning: facial detection and algorithmic bias.

### What exactly do we mean when we say a classifier is biased?

We'll be using the sizable, well curated CelebA dataset (as well as ImageNet) to train our facial detection classifiers, then testing them on a separate test dataset to determine their accuracy. To demonstrate that our model is free from any unintentional bias, we set out to develop a model that trains on CelebA and performs well across all demographics on the test dataset.

When we refer to a classifier as biassed, what do we exactly mean? We must consider latent variables, which characterise a dataset but are not rigorously observed, in order to formalise this. We will refer to the probability distributions of the aforementioned latent variables as the latent space. Combining these concepts, we define a classifier as biassed if, after seeing some more latent features, its classification decision changes.

Building a facial detection model that learns the latent variables underlying face image datasets and uses them to adaptively re-sample the training data, mitigating any biases that may be present in order to train a debiased model, is an exploration into a recently published method for addressing algorithmic bias.
