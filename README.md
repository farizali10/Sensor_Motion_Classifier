# Sensor Motion Classifier

## Overview

The Sensor Motion Classifier is a data science project focusing on activity recognition using wireless sensor data. The goal is to predict user activities, such as walking, sitting, and bending, based on measurements from wireless sensors placed on the chest and ankles.

## Data

### Format

- The data is provided in CSV format.
- Each CSV file (named datasetID.csv) corresponds to one repetition of an activity.
- Columns in each file represent time steps, with information such as avg_rss12, var_rss12, avg_rss13, var_rss13, avg_rss23, and var_rss23.

### Temporal Information

- The dataset focuses on 250-millisecond intervals.
- Within each interval, 5 samples are taken per second (sampled at 20 Hz).
- Temporal sequences are collected for activities, providing a detailed look at the user's movements.

## Project Structure

- `src/`: Contains the source code for the Sensor Motion Classifier.
- `data/`: Placeholder for the dataset. Download and place the dataset here.
- `notebooks/`: Jupyter notebooks for exploration, analysis, and model development.

## Installation

1. Clone the repository.
   ```bash
   git clone https://github.com/yourusername/sensor-motion-classifier.git
   cd sensor-motion-classifier
   ```

2. Install dependencies.
   ```
   pip install -r requirements.txt
   ```
## Usage
1. Download the dataset and place it in the data/ directory.
2. Explore the Jupyter notebooks in the notebooks/ directory for data analysis and model development.
3. Run the main script for training and evaluating the model.
```
python src/main.py
```
## Bending Activities
- Two types of bending activities are considered, as illustrated in the provided figure.
- Sensor positions on the body (chest and ankles) are shown in the sensorsPlacement.pdf figure.

## Dataset Details
- The dataset contains 480 sequences.
- Each sequence has 42240 instances (individual data points).
  
## Feature Extraction
- Time-domain features are extracted from raw data to compress time series, reduce noise, and eliminate correlations.
- Features include mean and standard deviation for each reciprocal RSS reading from worn WSN sensors.
  
## Contribution Guidelines
Feel free to contribute by:
- Reporting issues.
- Submitting feature requests.
- Forking the repository and creating pull requests.
   
