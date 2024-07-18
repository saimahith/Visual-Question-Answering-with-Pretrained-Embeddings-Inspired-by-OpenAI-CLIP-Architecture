# Visual-Question-Answering-with-Pretrained-Embeddings-Inspired-by-OpenAI-CLIP-Architecture

## Objective 
Leveraging pretrained models to generate embeddings for the Visual Question Answering (VQA) task, converting it into a classification problem with a simplified answer space of 30 classes using the DAQUAR datase.

### Methodology
Utilized a ResNet-50 model pretrained on ImageNet to extract image embeddings before the classification head.
Employed the sentence transformer all-MiniLM-L6-v2 to extract textual embeddings.
Implemented a dual-encoder architecture for images and text, combining their embeddings via a linear layer with ReLU activation for dimensionality reduction, followed by concatenation and classification through a linear classifier.

####
