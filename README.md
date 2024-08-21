# Power Price Forecasting Project (Development Paused)

## Introduction
This project aims to forecast power prices in Norway using machine learning techniques. The project demonstrates a good workflow for a data scientist, including data collection, cleaning, processing, model training, evaluation, and visualization.

## Project Structure
- `data/`: Contains raw and processed data files.
- `notebooks/`: Jupyter notebooks documenting the process.
- `src/`: Source code for data collection, processing, and modeling.
- `models/`: Trained models and model-related files.
- `README.md`: Project documentation.
- `.gitignore`: Git ignore file.

## Setup Instructions

### Prerequisites
- Ubuntu on WSL2 (Windows 11)
- Python 3.8+
- Virtual Environment (`venv`)

### Installation
1. Create and activate a virtual environment:
    ```sh
    python3 -m venv PPP_env
    source PPP_env/bin/activate
    ```
    
2. Clone the repository:
    ```sh
    git clone git@github.com:Jon-Bull/PowerPricePrediction.git
    cd PowerPricePrediction
    ```
    
3. Install the required packages:
    ```sh
    pip install -r requirements.txt
    ```

## Data Collection
Data is collected from the following APIs:
- **Power Prices**: [NVE API](https://api.nve.no/doc/)
- **Weather Data**: OpenWeatherMap, Yr (Norwegian Meteorological Institute)

## Running the Project
1. **Data Collection**:
    ```sh
    python src/data_collection.py
    ```

2. **Data Cleaning**:
    ```sh
    python src/data_cleaning.py
    ```

3. **Model Training**:
    ```sh
    python src/model_training.py
    ```

4. **Model Evaluation**:
    ```sh
    python src/model_evaluation.py
    ```

## Results
Results and visualizations can be found in the `notebooks/` directory and the `reports/` directory.

## License
This project is licensed under the MIT License.
