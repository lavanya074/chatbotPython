# Chatbot Using Python

A simple AI chatbot built using Python, Natural Language Processing, and Deep Learning.

This chatbot is trained on predefined intents and can understand user messages, classify them into categories, and return suitable responses.

## Project Description

This project demonstrates how to build a basic chatbot using NLP and a neural network model. The chatbot reads user input, processes the text, predicts the intent using a trained model, and gives a response based on the matched intent.

The chatbot is trained using an `intents.json` file that contains different patterns and responses.

## Features

- Text-based chatbot
- Intent classification
- NLP-based text preprocessing
- Tokenization and lemmatization using NLTK
- Bag-of-words model for feature extraction
- Deep learning model using TensorFlow/Keras
- Predefined responses from JSON intents
- Trained model saved for reuse
- Console-based user interaction

## Technologies Used

- Python
- NLTK
- TensorFlow
- Keras
- NumPy
- JSON
- Pickle

## Project Structure

```text
chatbotPython/
│
├── chatbot.py
├── training.py
├── intents.json
├── chatbot_model.h5
├── chatbot_model.keras
├── words.pkl
├── classes.pkl
└── README.md
```

## Files Description

### `intents.json`

Contains the training data for the chatbot. It includes:

- Tags
- User input patterns
- Bot responses

Example intent categories include:

- Greetings
- Goodbye
- Age
- Name
- Shop
- Hours
- Programming
- Resources

### `training.py`

This file is used to train the chatbot model.

It performs:

- Loading intents from JSON
- Tokenizing words
- Lemmatizing words
- Creating training data
- Building a neural network model
- Training the model
- Saving the trained model

### `chatbot.py`

This file runs the chatbot.

It performs:

- Loading the trained model
- Loading words and classes
- Processing user input
- Predicting the intent
- Selecting a suitable response
- Displaying the chatbot response in the console

## Installation

1. Clone the repository:

```bash
git clone https://github.com/lavanya074/chatbotPython.git
```

2. Navigate to the project folder:

```bash
cd chatbotPython
```

3. Install the required libraries:

```bash
pip install numpy nltk tensorflow
```

4. Download required NLTK packages:

```python
import nltk
nltk.download('punkt')
nltk.download('wordnet')
```

## How to Train the Model

Run the training file:

```bash
python training.py
```

This will train the chatbot model and generate model files such as:

```text
chatbot_model.keras
words.pkl
classes.pkl
```

## How to Run the Chatbot

After training the model, run:

```bash
python chatbot.py
```

The chatbot will start in the terminal.

Example:

```text
GO! Bot is running!
hello
Hello!
what is your name?
You can call me yoko!
bye
Goodbye!
```

## How It Works

1. The chatbot reads user input.
2. The input sentence is tokenized.
3. Words are lemmatized to their root form.
4. A bag-of-words array is created.
5. The trained neural network predicts the intent.
6. The chatbot selects a response from `intents.json`.
7. The response is displayed to the user.

## Model Architecture

The chatbot uses a Sequential neural network model with:

- Dense layer
- Dropout layer
- Dense hidden layer
- Output layer with Softmax activation

The model is trained using categorical cross-entropy loss and SGD optimizer.

## Skills Demonstrated

- Python programming
- Natural Language Processing
- Deep Learning basics
- Neural network model training
- Intent classification
- JSON data handling
- Model saving and loading
- Console application development

## Future Improvements

- Add a graphical user interface
- Add speech recognition
- Add text-to-speech response
- Improve the dataset with more intents
- Add real-time learning capability
- Deploy as a web chatbot using Flask or Django
- Connect chatbot with a database
- Add better error handling

## Author
**Lavanya**

## License

This project is open-source and available for learning and development purposes.
