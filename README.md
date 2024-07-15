# Chatbot with Flask and PyTorch

This project implements a simple chatbot using Flask for the web interface and PyTorch for the deep learning model. The chatbot is trained to recognize user intents and provide appropriate responses.

## Features
- **Flask Web Interface**: Provides a web-based interface for user interaction.
- **Pre-trained PyTorch Model**: Utilizes a neural network trained on a set of predefined intents and responses.
- **Natural Language Processing**: Uses tokenization and bag-of-words techniques to process user input.
- **Dynamic Response Generation**: Predicts user intents and generates responses based on model confidence.

## Getting Started

### Prerequisites
- Python 3.x
- Flask
- PyTorch
- NLTK

### Installation
1. Clone the repository:
    ```bash
    git clone https://github.com/yourusername/chatbot-flask-pytorch.git
    ```
2. Navigate to the project directory:
    ```bash
    cd chatbot-flask-pytorch
    ```
3. Install the required packages:
    ```bash
    pip install -r requirements.txt
    ```
4. Download NLTK data:
    ```python
    import nltk
    nltk.download('punkt')
    ```

### Running the Application
1. Ensure you have the `intents.json` file with predefined intents and responses.
2. Train the model using the provided script (optional if you have the `data.pth` file):
    ```bash
    python train.py
    ```
3. Run the Flask application:
    ```bash
    python app.py
    ```
4. Open your browser and navigate to `http://127.0.0.1:5000/`.

## Project Structure
- `app.py`: Main Flask application file.
- `model.py`: Defines the neural network model.
- `nltk_utils.py`: Utility functions for NLP tasks.
- `train.py`: Script for training the neural network model.
- `intents.json`: JSON file containing predefined intents and responses.
- `data.pth`: File to save/load the trained model.

## How It Works
1. **Training**: The `train.py` script trains a neural network on the provided intents and saves the model.
2. **Inference**: The Flask application loads the trained model and processes user inputs to predict intents and generate responses.
3. **NLP Processing**: Utilizes tokenization and bag-of-words for converting user input into a format suitable for the model.

## Future Improvements
- Implement more advanced NLP techniques.
- Add more intents and responses.
- Improve the web interface with better design and functionality.

## License
This project is licensed under the MIT License. See the LICENSE file for details.

## Acknowledgements
- [Flask](https://flask.palletsprojects.com/)
- [PyTorch](https://pytorch.org/)
- [NLTK](https://www.nltk.org/)

Feel free to contribute to this project by submitting issues or pull requests. Happy coding!
