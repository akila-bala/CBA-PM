# Customer Behavior Analysis and Predictive Modeling in Supermarket Retail

![Python](https://img.shields.io/badge/Python-3.8%2B-blue)
![Jupyter Notebook](https://img.shields.io/badge/Jupyter-Notebook-orange)
![Data Mining](https://img.shields.io/badge/Data%20Mining-Project-green)
![IEEE](https://img.shields.io/badge/IEEE-Published-blue)

This project was developed during the Data Mining course at the [Department of Computer Science](https://chennai.vit.ac.in/) at [Vellore Institute of Technology](https://chennai.vit.ac.in/) under the supervision of Dr. Kavitha Dhanushkodi

Publication
This project has been published and is available on IEEE Xplore: [Customer Behavior Analysis and Predictive Modeling in Supermarket Retail](https://ieeexplore.ieee.org/document/10542125)

This repository contains a comprehensive data mining approach for analyzing customer behavior and building predictive models within the supermarket retail domain. The goal is to leverage advanced data analytics techniques to optimize business strategies and enhance profitability.

## Table of Contents

- [Introduction](#introduction)
- [Features](#features)
- [Installation](#installation)
- [Usage](#usage)
- [Project Structure](#project-structure)
- [Algorithms Implemented](#algorithms-implemented)
- [Innovations](#innovations)
- [Limitations](#limitations)
- [Future Work](#future-work)
- [Contributing](#contributing)
- [License](#license)

## Introduction

Understanding customer behavior is crucial for supermarkets to optimize their business strategies and improve profitability. This project uses machine learning techniques to analyze customer data and build predictive models that provide valuable insights into customer behavior. The models can help in customer segmentation, personalized marketing, inventory management, dynamic pricing, and more.

## Features

- Data preprocessing and exploratory data analysis
- Feature engineering
- Implementation of Support Vector Classifier (SVC) and Neural Networks
- Real-time customer segmentation and dynamic pricing models
- Integration of multi-source data for comprehensive analysis
- Explainable AI techniques for model interpretability

## Installation

1. Clone the repository:
    ```bash
    git clone https://github.com/your-username/supermarket-customer-analysis.git
    cd supermarket-customer-analysis
    ```

2. Create and activate a virtual environment:
    ```bash
    python -m venv venv
    source venv/bin/activate  # On Windows, use `venv\Scripts\activate`
    ```

3. Install the required dependencies:
    ```bash
    pip install -r requirements.txt
    ```

## Usage

1. Prepare the dataset with RFM features (Recency, Frequency, Monetary) as input variables and customer segments as the target variable.
2. Split the dataset into training and testing sets.
3. Train the SVC and Neural Network models using the provided training functions.
4. Evaluate the models on the test set to assess their performance.

Example script to train and evaluate the models:

```python
from model import train_svc, train_neural_network, evaluate_model

# Load and preprocess data
data = load_data('path/to/dataset.csv')
train_data, test_data = split_data(data)

# Train models
svc_model = train_svc(train_data)
nn_model = train_neural_network(train_data)

# Evaluate models
evaluate_model(svc_model, test_data)
evaluate_model(nn_model, test_data)
```

## Project Structure

```
supermarket-customer-analysis/
├── data/                     # Data files
├── notebooks/                # Jupyter notebooks for experimentation
├── src/                      # Source code
│   ├── data_preprocessing.py # Data preprocessing scripts
│   ├── feature_engineering.py# Feature engineering scripts
│   ├── model.py              # Model training and evaluation scripts
│   └── utils.py              # Utility functions
├── README.md                 # Project README file
└── requirements.txt          # Required Python packages
```

## Algorithms Implemented

### Support Vector Classifier (SVC)

```text
Algorithm 1: Support Vector Classifier (SVC)
Input: 
    - Training dataset with RFM features
    - Hyperparameters for SVC
Output:
    - Trained SVC model
Method:
1: Load and preprocess the dataset
2: Split the dataset into training and testing sets
3: Define the SVC model with specified hyperparameters
4: Train the SVC model on the training dataset
5: Evaluate the model on the test dataset
6: Return the trained model
```

### Neural Network

```text
Algorithm 2: Neural Network
Input: 
    - Training dataset with RFM features
    - Hyperparameters and architecture for the neural network
Output:
    - Trained Neural Network model
Method:
1: Load and preprocess the dataset
2: Split the dataset into training and testing sets
3: Define the neural network architecture
4: Train the neural network on the training dataset
5: Evaluate the model on the test dataset
6: Return the trained model
```

## Innovations

- **Integration of Multi-Source Data**
- **Real-Time Customer Segmentation**
- **Advanced Feature Engineering**
- **Hybrid Modeling Approaches**
- **Explainable AI Techniques**
- **Personalized Marketing Strategies**
- **Optimized Inventory Management**
- **Dynamic Pricing Models**
- **Cross-Sell and Up-Sell Opportunities**
- **Customer Churn Prediction**

## Limitations

This model has been trained on a sample dataset and the performance is limited by the computational resources available. Higher accuracy can be achieved with larger datasets and more powerful computing infrastructure. Additionally, the model's ability to generalize to different supermarket environments may require further adaptation and fine-tuning.

## Future Work

- Enhance the model by incorporating more complex features and larger datasets.
- Explore the use of other advanced machine learning techniques for improved performance.
- Implement real-time data processing and prediction for dynamic customer behavior analysis.
- Extend the study to include more diverse retail environments and customer demographics.

## Contributing

Contributions are welcome! Please submit a pull request or open an issue to discuss potential changes.

## License

This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for details.
