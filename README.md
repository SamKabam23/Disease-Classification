# Disease-Classification

This project utilizes deep learning techniques to classify diseases from medical images. By leveraging convolutional neural networks (CNNs), the model is trained to achieve high accuracy in disease prediction. The project integrates MLOps practices and supports cloud deployments, ensuring robust performance in production environments.

## Table of Contents
- [Introduction](#introduction)
- [Features](#features)
- [Installation](#installation)
- [Usage](#usage)
- [Project Structure](#project-structure)
- [Model Training](#model-training)
- [Evaluation](#evaluation)
- [Deployment](#deployment)
- [Contributing](#contributing)
- [License](#license)

## Introduction
This Disease Classification project aims to enhance healthcare by providing an automated system for disease detection from medical images. It employs advanced machine learning techniques to analyze images and identify potential diseases, supporting early diagnosis and treatment.

## Features
- **Deep Learning Model:** Utilizes CNN for high-accuracy image classification.
- **Data Pipeline:** Automated data ingestion and preprocessing for seamless workflow.
- **MLOps Integration:** Supports DVC for dataset and model checkpoint version control.
- **Cloud Deployment:** Configurable for deployment on various cloud platforms.
- **Evaluation Metrics:** Comprehensive performance evaluation and visualization tools.

## Installation
1. **Clone the repository:**
    ```bash
    git clone https://github.com/SamKabam23/Disease-Classification.git
    cd Disease-Classification
    ```

2. **Install dependencies:**
    ```bash
    pip install -r requirements.txt
    ```

3. **Set up DVC:**
    ```bash
    dvc init
    dvc pull
    ```

## Usage
1. **Data Ingestion:**
    Place your data in the `artifacts/data_ingestion` directory.

2. **Configuration:**
    Update the `config/config.yaml` file with your dataset paths and model parameters.

3. **Train the Model:**
    ```bash
    python main.py train
    ```

4. **Evaluate the Model:**
    ```bash
    python main.py evaluate
    ```

## Project Structure
```
Disease-Classification/
├── artifacts/
│   └── data_ingestion/
├── config/
│   └── config.yaml
├── research/
├── src/
│   └── cnnClassifier/
├── templates/
├── .gitignore
├── dvc.yaml
├── LICENSE
├── main.py
├── params.yaml
├── README.md
├── requirements.txt
├── setup.py
└── template.py
```

## Model Training
The model training process, managed by `main.py`, reads configurations from `config.yaml` and trains the CNN model using the specified dataset. The process includes data augmentation, model checkpointing, and logging.

## Evaluation
The evaluation script provides key metrics such as accuracy, precision, recall, and F1-score. It also generates confusion matrices and ROC curves for detailed performance analysis.

## Deployment
Designed for cloud deployment, the project configuration in `dvc.yaml` ensures efficient model versioning and data dependency management.

## Contributing
Contributions are welcome! Please follow these steps:
1. Fork the repository.
2. Create a new branch (`git checkout -b feature-branch`).
3. Commit your changes (`git commit -m 'Add new feature'`).
4. Push to the branch (`git push origin feature-branch`).
5. Create a new Pull Request.

## License
This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for details.