# Housing Price Regression Project

This project aims to predict housing prices using various regression models. The models are trained on a dataset containing housing features and are evaluated based on mean absolute error, mean squared error, and R-squared score.

## Demo Video

[Watch the demo video](https://youtu.be/LU1fTtT395k)

## Setup and Installation

1. **Clone the repository:**

    ```bash
    git clone https://github.com/yourusername/regression_project.git
    cd regression_project
    ```

2. **Install the required packages:**

    ```bash
    pip install -r requirements.txt
    ```

3. **Run the `model_training.py` script to train and save the models:**

    ```bash
    python model_training.py
    ```

4. **Start the Flask application:**

    ```bash
    python app.py
    ```

## Usage

- Navigate to `http://127.0.0.1:5000/` in your web browser.
- Select a model and enter the required features to predict the housing price.
- View the prediction result on the results page.

## Front End User Input Interface

![Front End User Input Interface](https://github.com/vineet-kumar-tennessee/regression/blob/main/housing_price_prediction/front_end_images/front_end_input.png)

This is how the front end user input interface looks like. The model will predict based on these user inputs.

## Evaluation

- The evaluation results of the models are displayed on the `/results` page.
- The models are evaluated based on Mean Absolute Error (MAE), Mean Squared Error (MSE), and R-squared (R2) score.

## Contributing

If you would like to contribute to this project, please fork the repository and submit a pull request.
