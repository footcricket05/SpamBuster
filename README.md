# SpamBuster: Email Spam Filtering System

## Overview
SpamBuster is an API that leverages a machine learning algorithm to predict whether an email ID is spam or not. When you pass an email ID as a parameter to this API, it responds with a boolean value (True/False) to indicate whether the email is considered spam or not.

## Dataset
To train the machine learning algorithm, we utilized a dataset available at [this link](https://archive.ics.uci.edu/ml/datasets/Spambase/). The dataset comprises 4,601 email messages, each associated with a set of attributes.

## Technical Details
SpamBuster is built using Python and the Flask framework for creating the API. We employed the Random Forest Classifier from the scikit-learn library for spam classification. The model is trained using the Spambase dataset.

## Usage
To use this project, you need to have Python installed on your system. Follow these steps:

1. Clone this repository and navigate to the project directory in your terminal.

2. Install the required dependencies using the following command:
   ```
   pip install -r requirements.txt
   ```

3. After installing the dependencies, start the API server with the following command:
   ```
   python app.py
   ```

The API server will run on http://localhost:5000/. You can send a GET request to http://localhost:5000/predict with the email ID as a parameter in the query string. For example:

```
http://localhost:5000/predict?email_id=hello@world.com
```

The API will respond with a boolean value, indicating whether the email ID is spam or not.

## Contributing
We welcome contributions! Please don't hesitate to submit a pull request or open an issue if you have suggestions or feedback.

## License
This project is licensed under the  `MIT License`. Refer to the LICENSE file for more details.
