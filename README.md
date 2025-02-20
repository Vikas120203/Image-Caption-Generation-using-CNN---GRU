# Image-Caption-Generation-using-CNN---GRU
Automatically generating human-like captions for images using deep learning (CNN-GRU). This project was published in an IEEE Conference and explores image captioning using a combination of Convolutional Neural Networks (CNN) and Gated Recurrent Units (GRU).
Published in: IEEE Conference
📌 Technologies Used: CNN (ResNet-50) + GRU for image captioning
📊 Evaluation Metrics: BLEU, METEOR, CIDEr
🗂️ Dataset: Flickr8k, Flickr30k


✨ Features
✅ End-to-End Deep Learning Pipeline (Image Processing → Feature Extraction → Caption Generation)
✅ CNN-GRU Model for accurate captioning
✅ Pretrained ResNet-50 for feature extraction
✅ Word Embeddings (GloVe - 300D) for text understanding
✅ Optimized with Adam Optimizer for better training stability
✅ Comparison with LSTM & RNN-based approaches
✅ BLEU-4 score of 0.421 (higher than CNN-LSTM)


📚 Dataset
We used two major datasets:

Flickr8k (8,000 images with 5 captions each)
Flickr30k (30,000 images with 5 captions each)
📸 Image Preprocessing:

Resized to 224×224 pixels
Normalized pixel values
Data Augmentation for better generalization

📝 Text Preprocessing:

Tokenization & Stemming
GloVe Embeddings for NLP
Sequence Padding for uniform input size
🏗 Methodology
1️⃣ CNN - Image Feature Extraction
We use ResNet-50 (a powerful CNN) to extract 2048-dimensional feature vectors from images.

2️⃣ GRU - Caption Generation
A Gated Recurrent Unit (GRU) processes image features and generates word-by-word captions.

3️⃣ Training & Optimization
Loss Function: Cross-Entropy Loss
Optimizer: Adam

Model perfomance:
Model	BLEU-1	BLEU-2	BLEU-3	BLEU-4	METEOR	CIDEr
CNN-GRU	0.743	0.614	0.506	0.421	0.332	0.652
CNN-LSTM	0.714	0.585	0.473	0.391	0.312	0.603
CNN-RNN	0.682	0.558	0.432	0.347	0.274	0.536

🏆 Key Insight:
CNN-GRU outperformed CNN-LSTM and CNN-RNN in all major NLP evaluation metrics!
