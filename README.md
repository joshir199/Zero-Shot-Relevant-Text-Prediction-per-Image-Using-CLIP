# Zero-Shot-Relevant-Text-Prediction-per-Image-Using-CLIP
Understanding the working and architecture of famous CLIP for predicting most relevant text given the image.

Classification by CLIP can be done by having a list of text embeddings corresponding to each class, and mapping it to image embeddings. 
These predictions are done in latent/abstraction space.


******************************
# Architecture

![](https://github.com/joshir199/Zero-Shot-Relevant-Text-Prediction-per-Image-Using-CLIP/blob/main/images/clip_architecture.png)



********************************
# Dataset details:

1. The above model was trained on 400 million image - text dataset.
2. The text/words used in the dataset was from limited vocabulary with size of 500,000 words.
3. Each text item used corresponding to image can have at most 76 token ( ~ 25 words).


**********************************
# Training details

1. Used ViT as Image Encoder and GPT-x (x ~ 2 or 3 ) as Text Encoder

2. Embedding dimension used for learning features is 512

3. The model was trained for around 2-3 weeks on around 250 V100 GPUs.


   
