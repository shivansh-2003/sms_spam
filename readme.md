# SMS/Email Spam Classifier

A simple, user-friendly application that helps you identify whether a message is spam or legitimate.

![Spam Classifier Demo](https://github.com/yourusername/sms_spam/raw/main/demo.png)

## What Does This Application Do?

This application analyzes text messages or emails and tells you if they're likely spam or not. It uses machine learning to make these predictions based on patterns it learned from thousands of real messages.

## Features

- Simple, easy-to-use interface
- Quick analysis of any message
- Clear "Spam" or "Not Spam" result
- Works with both SMS messages and emails

## Getting Started

### Prerequisites

Before you can use this application, you need to have the following installed on your computer:

- Python 3.7 or higher ([Download Python](https://www.python.org/downloads/))
- Git (optional, for cloning the repository) ([Download Git](https://git-scm.com/downloads))

### Installation

Follow these simple steps to get the application running on your computer:

1. **Download or clone this repository**

   Download the ZIP file and extract it, or if you have Git installed, run:
   ```
   git clone https://github.com/yourusername/sms_spam.git
   cd sms_spam
   ```

2. **Set up a virtual environment (recommended but optional)**

   On Windows:
   ```
   python -m venv venv
   venv\Scripts\activate
   ```

   On macOS/Linux:
   ```
   python3 -m venv venv
   source venv/bin/activate
   ```

3. **Install required packages**

   ```
   pip install -r requirements.txt
   ```

4. **Download NLTK data**

   Run Python in your terminal/command prompt:
   ```
   python -c "import nltk; nltk.download('punkt'); nltk.download('stopwords')"
   ```

### Running the Application

1. **Start the application**

   ```
   streamlit run app.py
   ```

2. **Access the application**

   Your web browser should automatically open to `http://localhost:8501`. If not, open your browser and navigate to this address.

## How to Use

1. Type or paste your message into the text box
2. Click the "Predict" button
3. The application will display "Spam" or "Not Spam" based on its analysis

## How It Works

This application uses:
- Natural Language Processing (NLP) to understand message content
- Text transformation techniques to prepare the text for analysis
- Machine learning algorithms to make predictions based on patterns in known spam messages

## Files in this Repository

- `app.py` - The main application code
- `model.pkl` - The trained machine learning model
- `vectorizer.pkl` - The text vectorizer that converts messages into a format the model can understand
- `requirements.txt` - List of Python packages needed to run the application

## Troubleshooting

**Problem**: The application won't start
- Make sure you've installed all requirements using `pip install -r requirements.txt`
- Ensure you've downloaded the required NLTK data

**Problem**: You get errors about missing files
- Verify that `model.pkl` and `vectorizer.pkl` are in the same directory as `app.py`

## Contributing

Feel free to fork this repository and submit pull requests to improve the application!

## License

This project is licensed under the MIT License - see the LICENSE file for details.

## Acknowledgments

- Thanks to everyone who contributed to the development of this spam classifier
- Special thanks to the creators of NLTK, Streamlit, and scikit-learn for their amazing tools
