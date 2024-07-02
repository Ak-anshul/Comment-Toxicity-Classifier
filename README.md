# Comment Toxicity Classifier using Deep Learning and NLP

This project involves building a deep learning model to classify the toxicity of comments. The model is trained to detect multiple types of toxicity, including toxic, severe toxic, obscene, threat, insult, and identity hate. The project utilizes a dataset of comments and employs various techniques in data preprocessing and model building.

## Dataset

The dataset used in this project is `Comment_Toxicity.csv`, which contains comments and their respective toxicity labels.

## Preprocessing

1. **Tokenization**: The text data is tokenized using `Tokenizer` from `tensorflow.keras.preprocessing.text`.
2. **Padding**: The tokenized sequences are padded to ensure uniform input length using `pad_sequences`.

## Model Architecture

The model is built using the following layers:
- **Embedding**: Transforms the input text into dense vectors of fixed size.
- **LSTM**: Captures the sequential dependencies in the data.
- **Dense Layers**: Three fully connected layers with ReLU activation to learn complex features.
- **Output Layer**: A dense layer with sigmoid activation for multi-label classification.

## Training

The model is trained on the preprocessed dataset with a training and validation split. The training involves 5 epochs, and the loss and accuracy are plotted for both training and validation data.

## Results

The model successfully identifies various types of toxicity in comments. The training and validation accuracy and loss plots indicate good model performance.

