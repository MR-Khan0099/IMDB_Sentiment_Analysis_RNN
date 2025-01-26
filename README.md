# IMDB Movie Review Sentiment Analysis


## Overview
This project implements a sentiment analysis application using a recurrent neural network (RNN) model trained on the IMDB dataset. The application predicts whether a given IMDB movie review expresses a positive or negative sentiment.

## Features
- Model Training: A custom simple RNN model is trained from scratch using the IMDB dataset.
- Sentiment Classification: Predicts whether a review sentiment is positive or negative.
- Interactive User Interface: Built with Streamlit for an intuitive web-based interface.
- Pre-trained Model Loading: The trained model is saved as imdb_Rnn.h5 for reuse.

## Installation
1. Clone the repository:
    ```bash
    git clone https://github.com/MR-Khan0099/IMDB_Sentiment_Analysis_RNN.git
    ```
2. Install the required dependencies:
    ```bash
    pip install -r requirements.txt
    ```
Example dependencies include:

TensorFlow
Streamlit
NumPy
    
3. Ensure the trained model (imdb_Rnn.h5) is available in the project directory. If not, you can generate it by running simpleRnn.ipynb.

## Usage
1. Start the Streamlit application:

```bash
streamlit run app.py 
```
Open the application in your browser at http://localhost:8501.

Enter a movie review in the provided text area and click Classify. The app will display:
Sentiment (Positive/Negative)
Prediction Score

## Workflow
1. Model Training:
The RNN is trained on the IMDB dataset.
Reviews are tokenized and padded to a fixed length of 500 for uniformity.

2. Prediction Pipeline:
The app processes user-input text into a model-compatible format.
The trained model generates predictions, indicating the sentiment score.

3. User Interface:
The web-based UI offers real-time, interactive sentiment analysis.

## Model Details
- Architecture: A simple RNN built with TensorFlow/Keras.
- Dataset: IMDB Movie Reviews Dataset.
- Training Parameters:
Activation function: ReLU
Loss function: Binary cross-entropy
Optimizer: Adam
Metrics: Accuracy

## Future Enhancements
- Add visualizations of review sentiment trends.
- Experiment with advanced models (e.g., LSTM, GRU) for improved performance.
- Integrate additional datasets for multi-class sentiment classification.



## License
This project is licensed under the MIT License. See the LICENSE file for details.
