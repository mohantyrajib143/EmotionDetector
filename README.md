# Emotion Detector

## Project Overview

The Emotion Detector is a Python-based web application that detects emotions expressed in a given text using the Watson Natural Language Processing (NLP) library.

The application analyzes text and identifies the following emotions:

- Anger
- Disgust
- Fear
- Joy
- Sadness

It also identifies the dominant emotion based on the detected emotion scores.

## Technologies Used

- Python
- Flask
- Watson NLP Library
- Requests
- Unittest
- PyLint
- HTML and CSS

## Project Structure

```text
EmotionDetector/
├── EmotionDetection/
│   ├── __init__.py
│   └── emotion_detection.py
├── server.py
├── test_emotion_detection.py
└── README.md
```

## Features

- Detects emotions from user-provided text.
- Identifies anger, disgust, fear, joy, and sadness.
- Determines the dominant emotion.
- Provides a web interface using Flask.
- Handles invalid or empty input.
- Includes unit tests to validate application functionality.
- Supports static code analysis using PyLint.

## Installation

1. Clone the repository:

   ```bash
   git clone <YOUR_GITHUB_REPOSITORY_URL>
   ```

2. Navigate to the project directory:

   ```bash
   cd <YOUR_PROJECT_DIRECTORY>
   ```

3. Install the required dependencies:

   ```bash
   pip install flask requests pylint
   ```

   Install any additional dependencies required by the Watson NLP service used in the implementation.

## Usage

Run the Flask application:

```bash
python3 server.py
```

Open your browser and navigate to:

```text
http://127.0.0.1:5000
```

Enter text into the application to detect the emotions expressed in the input.

## Running Unit Tests

Execute the unit tests using:

```bash
python3 -m unittest test_emotion_detection.py
```

## Static Code Analysis

Run PyLint on the Flask server:

```bash
pylint server.py
```

## Error Handling

The application handles empty input and unsuccessful requests to the emotion detection service to prevent unexpected application behavior.

## Expected Output

For valid text input, the application returns a dictionary containing the scores for the five emotions and the dominant emotion.

Example structure:

```python
{
    'anger': 0.01,
    'disgust': 0.01,
    'fear': 0.01,
    'joy': 0.95,
    'sadness': 0.01,
    'dominant_emotion': 'joy'
}
```

*Note: The scores above are illustrative. Actual results depend on the input text and the NLP service response.*

## Author

Developed as part of the Coursera Python-based AI web application development final project.
