# Diet Recommendation System-Machine Learning project

The **Diet Recommendation System** is a machine learning-based project designed to provide personalized dietary recommendations. It calculates essential metrics like BMI, BMR, and daily caloric needs, and utilizes clustering to recommend foods based on nutritional requirements and user preferences. 

## Features

- **Caloric Maintenance Prediction**: Uses Linear Regression to estimate calories needed for weight maintenance.
- **Weight Change Planning**: Calculates daily caloric needs for achieving desired weight goals over a given timeframe.
- **Food Clustering and Recommendation**: Clusters food items using K-Means and recommends similar items based on a target food.
- **Visualization**: Provides insights through feature importance and nutritional breakdown visualizations.

## Dataset

1. **Primary Dataset**: `Dataset.csv`  
   This dataset contains information about user demographics and activity levels, used to predict caloric requirements.

2. **Secondary Dataset**: `RAW_recipes.csv`  
   The dataset includes food recipes and nutritional information, used for clustering and recommendation.  
   Access it [here](https://www.kaggle.com/datasets/shuyangli94/food-com-recipes-and-user-interactions?select=RAW_recipes.csv).

## Installation

### Option 1: Local Installation

1. Clone the repository:
   ```bash
   git clone <repository-url>
   cd <repository-directory>
   ```

2. Install the required dependencies:
   ```bash
   pip install -r requirements.txt
   ```

3. Open the Jupyter Notebook:
   ```bash
   jupyter notebook Diet_Recommendation_System.ipynb
   ```

### Option 2: Using Docker

1. Build the Docker image:
   ```bash
   docker build -t diet-recommendation .
   ```

2. Run the container:
   ```bash
   docker run diet-recommendation
   ```

## Usage

1. **Data Preprocessing**: The notebook cleans and preprocesses the datasets for machine learning and clustering.
2. **Model Training**: Linear Regression is trained on user demographic data to predict caloric maintenance requirements.
3. **Recommendation**: Provide user inputs to get tailored dietary recommendations for different meal times.

## File Structure

- `Diet_Recommendation_System.ipynb`: Main Jupyter Notebook containing the code and implementation.
- `Diet_Recommendation_System.py`: Python script version of the notebook.
- `Dataset.csv`: Primary dataset for caloric maintenance prediction.
- `RAW_recipes.csv`: Dataset for food clustering and recommendation.
- `requirements.txt`: List of dependencies.
- `Dockerfile`: Configuration for containerizing the application.