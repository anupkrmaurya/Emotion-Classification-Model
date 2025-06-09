Emotion Classification using Deep Learning

Project Overview
This project is an emotion classification model that uses deep learning (TensorFlow/Keras) to predict emotional tone (e.g., joy, anger, sadness, fear, etc.) from raw text input. It is deployed using Gradio for a live interactive demo and includes key evaluation metrics like confusion matrix, accuracy plots, and a classification report.

Dataset Used

File: training.csv

- Columns:
  - text – Input sentence or statement.
  - label – Corresponding emotion label (encoded as integers).
- Format: Supervised, labeled data.
- Classes (Example): 
  - 0: Sad
  - 1: Happy
  - 2: Love  
  - 3: Anger  
  - 4: Fear  

Model Approach

1. Text Preprocessing
- Tokenized using Tokenizer()
- Padded with pad_sequences to uniform length

2. Model Architecture
Embedding Layer → Flatten → Dense (ReLU) → Dense (Softmax)

3. Training
- Optimizer: Adam
- Loss: Categorical Crossentropy
- Metric: Accuracy
- Split: 80% training, 20% testing

4. Evaluation
- Accuracy & loss curves across epochs
- Classification report (Precision, Recall, F1-score)
- Confusion matrix for multiclass performance

5. Deployment
- Live demo using Gradio
- Link auto-generated in Colab using share=True

Visualizations

- Epoch-wise accuracy and loss plots  
- Confusion matrix using Seaborn  
- Classification report with all key metrics  
- Gradio-based UI for interactive testing

Creativity Highlights

- Included an intuitive Gradio UI with example inputs
- Designed the model with expandability in mind (can easily scale to more emotions)
- User-friendly explanations and interface
- Visualization of metrics to help interpret results clearly

Dependencies

pip install tensorflow keras gradio seaborn matplotlib scikit-learn pandas numpy

Run Instructions (Colab)

1. Upload training.csv to your Colab runtime.
2. Copy the provided notebook blocks into cells.
3. Run the entire notebook.
4. Interact with the model via Gradio UI link.
