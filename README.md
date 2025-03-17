# Health Score Prediction and AI Agent

## Overview
This repository contains a machine learning pipeline designed to predict health scores and integrate the predictions into an AI agent that provides personalized health recommendations. The pipeline includes data preprocessing, model development, hyperparameter tuning, and an LLM-powered AI agent enhanced with retrieval-augmented generation (RAG).

## Project Structure
- **Data Preprocessing**: Cleaning and preparing the dataset, handling missing values, and conducting exploratory data analysis (EDA).
- **Machine Learning Model**: Predicting health scores using an XGBoost model with hyperparameter tuning and cross-validation.
- **LLM Integration**: Generating embeddings from the cleaned dataset and testing different LLMs to select the best-performing model.
- **AI Agent Development**: Implementing an AI agent using RAG and prompt engineering to enhance response accuracy with scientific literature.

## Implementation Details
### 1. Data Preprocessing
- Loaded and cleaned the dataset, ensuring data quality by handling missing values.
- Performed classic exploratory data analysis (EDA) to understand data distributions and patterns.

### 2. Machine Learning Model
- Selected **health score** as the target variable.
- Experimented with **Random Forest** and **XGBoost**, with XGBoost performing better overall.
- Used **grid search** to find the best hyperparameters for the XGBoost model.
- Implemented **5-fold cross-validation** to prevent overfitting and improve generalization.

### 3. LLM Integration
- Created **RAG embeddings** from the cleaned dataset to enhance LLM performance.
- Evaluated multiple LLMs:
  - **GPT-4**
  - **Med-Alpaca**
  - **BioMedLM**
- Found that **GPT-4** provided the most reliable results for the given use case.

### 4. AI Agent Development
- Developed an AI agent using **N-10** for user input handling.
- Conducted **prompt engineering** to improve the model's responses.
- Integrated additional **scientific and medical literature** into the RAG system.
- Ensured that the agent consults **RAG embeddings** before providing answers to improve accuracy.

## Current Status
The final model is deployed with:
- **XGBoost** as the predictive model for health scores.
- **GPT-4** as the selected LLM for generating health recommendations.
- **RAG-enhanced AI agent** with scientific literature integration for improved accuracy.

This version represents the most refined and effective model to date, ready for further enhancements as needed.

## Future Improvements
- Expanding the dataset for improved generalization.
- Experimenting with additional fine-tuned LLMs for specific medical use cases.
- Enhancing the AI agent’s ability to interact dynamically with users.

## How to Use
1. Clone this repository.
2. Follow the installation steps (to be provided in a separate setup guide).
3. Run the preprocessing script to clean and prepare the dataset.
4. Train the XGBoost model using the hyperparameter-tuned settings.
5. Deploy the AI agent with integrated RAG embeddings and prompt engineering.
6. Interact with the AI agent for personalized health recommendations.

## Contributing
Contributions are welcome! Please open an issue or submit a pull request with any enhancements or bug fixes.




