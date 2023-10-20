# Credit Scoring Dashboard and API

This repository contains the code for a machine learning-powered Credit Scoring Dashboard and API developed for the "Prêt à dépenser" financial company. The project aims to predict the probability of credit default for potential clients, facilitate transparent decision-making, and provide insights for relationship managers.

## Table of Contents

- [Features](#features)
- [Getting Started](#getting-started)
  - [Prerequisites](#prerequisites)
  - [Installation](#installation)
- [Usage](#usage)
  - [Dashboard](#dashboard)
  - [API](#api)
- [File Structure](#file-structure)
- [Contributing](#contributing)
- [License](#license)

## Features

- **Dashboard**: Interactive web application built with Streamlit, providing relationship managers with the ability to evaluate a client's credit score, view client information, and explore model predictions visually.
- **API**: Flask-based API for retrieving credit scoring predictions programmatically.
- **Data Drift Detection**: Utilizes Evidently library to detect data drift between training and production datasets.
- **Custom Scoring Metric**: Implements a custom scoring metric, F10Score, to account for business-specific constraints.
- **Model Optimization**: Uses Optuna for hyperparameter optimization and handles class imbalance using class weights and probability threshold tuning.

## Getting Started

### Prerequisites

- Python 3.7 or higher
- Install required packages using `pip install -r requirements.txt`

### Installation

1. Clone the repository:

   ```bash
   git clone https://github.com/your-username/credit-scoring-dashboard.git
   ```

2. Change directory to the project folder:

   ```bash
   cd credit-scoring-dashboard
   ```

3. Install dependencies:

   ```bash
   pip install -r requirements.txt
   ```

## Usage

### Dashboard

#### Installation

1. Clone the repository:

   ```bash
   git clone https://github.com/YassineR/P7.git
   ```

2. Change directory to the project folder:

   ```bash
   cd credit-scoring-dashboard
   ```

3. Install dependencies:

   ```bash
   pip install -r requirements.txt
   ```
To run the interactive dashboard, execute the following command:

#### Run
```bash
streamlit run dashboard.py
```

Access the dashboard at `http://localhost:8501` in your web browser.

### API
#### Installation

1. Clone the repository:

   ```bash
   git clone https://github.com/YassineR/P7-backend.git
   ```

2. Change directory to the project folder:

   ```bash
   cd credit-scoring-dashboard
   ```

3. Install dependencies:

   ```bash
   pip install -r requirements.txt
   ```
To run the interactive dashboard, execute the following command:

#### Run
To start the Flask API, run:

```bash
python app.py
```

The API will be accessible at `http://localhost:5000`. Refer to the API documentation for endpoint details.

## File Structure

- **P7/**
  - **dashboard.py**: Streamlit application for the interactive dashboard.
  - **home_credit_data_sample.csv**: Sample preprocessed data for demonstration.
  - **logo.png**: Project logo used in the dashboard.
  - **model.pkl**: Serialized LightGBM model for credit scoring.
  - **requirements.txt**: List of Python dependencies.
  - **tools.py**: Utility functions for generating visualizations.
- **P7-backend/**
  - **app.py**: Flask-based API for credit scoring predictions.
  - **lgbm_client_scoring.pkl**: Serialized LightGBM model for the API.
  - **requirements.txt**: List of Python dependencies for the API.
  - **tests/**
    - **test_app.py**: Unit tests for API endpoints.

## Contributing

Contributions are welcome! Please open an issue or create a pull request to discuss changes or additions.

## License

This project is licensed under the [MIT License](LICENSE).
