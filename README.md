# Real vs Fake Image Tests

Evaluate open source models in their detection of real vs fake images of people. Here, we test the following models:

- **dima806/deepfake_vs_real_image_detection**: This model is an image classifier that generates real vs fake scores. No explanations are provided.
- **Wvolf/ViT_Deepfake_Detection**: This model is an image classifier that generates real vs fake scores. No explanations are provided.
- **umm-maybe/AI-image-detector**: This model is an image classifier that generates human vs artificial scores. No explanations are provided.
- **meta-llama/Llama-3.2-11B-Vision-Instruct**: This model is a general purpose image model that generates real vs fake scores as well as explanations.

## Dataset
The dataset for this test is the [Roboflow Image Detection (Rake & Real) Dataset v1](https://universe.roboflow.com/1-3wzs6/image-detection-fake-real/dataset/1). Here, we test only a small sample to demonstrate proof-of-concept. Note that other image datasets, such as the [Kaggle 140k Real and Fake Faces](https://www.kaggle.com/datasets/xhlulu/140k-real-and-fake-faces) dataset may be used in future tests.

## Process
The testing process comprises the following steps:
- Randomly select sample a set of real and fake images to serve as test dataset.
- For each image in test dataset:
  - For each model:
      - Generate real and fake scores for image.
      - Compare real and fake scores against the actual image type (i.e., Real vs Fake).
- Show performance of each model for each image.

## Test


