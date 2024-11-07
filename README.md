# Pose Detection with Transformer and Ensemble Models

This repository contains code and models for detecting poses in videos using a Transformer-based model and an ensemble approach. The project aims to process sequences of frames, extract meaningful features, and leverage sequential modeling to improve pose detection accuracy. While promising, current results indicate further refinement is needed to achieve practical classifier performance.

## Data Source

The data used in this project was sourced from the following Kaggle dataset:

[Workout Fitness Video Dataset](https://www.kaggle.com/datasets/hasyimabdillah/workoutfitness-video/data?source=post_page-----7f8972ee8370--------------------------------)

This dataset contains various workout and fitness videos, which were processed and used for pose detection and sequence analysis.

## Project Overview

This project explores different machine learning models and architectures for pose detection in video data, specifically:
- **Feature Engineering**: Extracting x, y, and z coordinates for each landmark in video frames.
- **Transformer Model**: Using a Transformer architecture for its ability to learn from sequential data and capture dependencies across frames.
- **Ensemble Modeling**: Stacking models by combining their predicted probabilities, with XGBoost as the meta-learner for improved accuracy.

## Key Features

1. **Data Processing**:  
   - Converts video frames into 99 features (x, y, z coordinates for 33 landmarks).
   - Creats additional distance and angle features to be used in conjunction with the 99 xyz features. 
   - Groups frames for consistent sequence lengths, padding videos with fewer frames.

2. **Modeling with Transformers**:  
   - A Transformer-based model captures temporal dependencies between landmarks across frames, showing promising accuracy on the task.


