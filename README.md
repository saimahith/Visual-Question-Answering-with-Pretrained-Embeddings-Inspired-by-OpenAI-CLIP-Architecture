# Visual-Question-Answering-with-Pretrained-Embeddings-Inspired-by-OpenAI-CLIP-Architecture

## Objective 
Leveraging pretrained models to generate embeddings for the Visual Question Answering (VQA) task, converting it into a classification problem with a simplified answer space of 30 classes using the DAQUAR datase.

### Methodology
Utilized a ResNet-50 model pretrained on ImageNet to extract image embeddings before the classification head.
Employed the sentence transformer all-MiniLM-L6-v2 to extract textual embeddings.
Implemented a dual-encoder architecture for images and text, combining their embeddings via a linear layer with ReLU activation for dimensionality reduction, followed by concatenation and classification through a linear classifier.

#### Architecture
![Screenshot_18-7-2024_105834_](https://github.com/user-attachments/assets/c2ea655c-277c-4eac-9d15-3484fac22432)
Visual Question Answering (VQA) model uses a dual-encoder architecture. The image encoder utilized a pretrained ResNet-50 model to extract image embeddings, while the text encoder used the all-MiniLM-L6-v2 sentence transformer for textual embeddings. Both embeddings were processed through a linear layer with ReLU activation for dimensionality reduction and then concatenated. The combined embeddings were fed into a linear classifier to generate the final answer. This architecture optimized computational efficiency and accuracy for the VQA task.
