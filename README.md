# Crypto Sentiment Analysis Using LoRA

## Project Overview

The influence of social media sentiment on financial markets is a significant factor, especially in volatile sectors like cryptocurrency. This project presents a sentiment classification framework designed to analyze and classify crypto-related tweets to detect financially relevant sentiment.

This work was conducted as part of a Master's program at Berkeley.

## The Problem

Traditional market analysis often misses the real-time public sentiment that can drive rapid price changes in cryptocurrency. The goal of this project was to develop a robust, efficient, and accurate framework for classifying the sentiment of crypto-related social media content, thereby providing a valuable data stream for financial decision-making.

## Methodology

### 1. Data Collection & Preprocessing
Tweets were collected from social media platforms, preprocessed, and filtered to ensure they were financially relevant to the cryptocurrency domain.

### 2. Labeling Strategy
A hybrid heuristic and score-based approach was used to label tweets as positive, neutral, or negative. This method was designed to create a high-quality dataset for *financial sentiment* in the context of **Cryptocurrencies** in informal settings, such as Social Media.

### 3. Model & Fine-Tuning
We utilized **BERTweet-large**, a transformer-based language model pre-trained on Twitter data, as our core classifier. To make the fine-tuning process efficient, we implemented **Low-Rank Adaptation (LoRA)**. This technique significantly reduces the number of trainable parameters, allowing us to achieve high performance with far less computational cost.

## Key Results & Impact

Our experiments demonstrated that our LoRA-enhanced model significantly outperformed a baseline classifier, achieving over **80% classification accuracy**.

This work highlights the potential of using efficient, domain-aware NLP models to capture real-time public sentiment. The framework provides a strong foundation for future applications, such as integration with market forecasting tools or algorithmic trading strategies.

## My Contributions

As a collaborator on this project, my primary contributions included:
* **Define Model Architecture**
* **BERTweet fine-tuning using LoRA**
* **Statistical Analysis in R**
* **Contributed to extraction of conclusions and paper construction**

## Getting Started

To replicate this project, you will need to:
1. Clone this repository.
2. Install the required dependencies using `pip install -r requirements.txt`.
3. Follow the instructions in the `notebooks/` directory to run the data preprocessing, model training, and evaluation steps.

The key documents for this project are:
1. **Sentiment_Analysis_for_Social_Media.pdf**: The paper that describes the theory, methods, and results of this project.
2. **Crypto_Sentiment_Analysis_BERTweet.ipynb**: The main notebook with the data discovery, the training of the baseline and LoRA models, and half of the iterations for hyperparameter optimization.
3. **Copy_Crypto_Sentiment_Analysis_BERTweet.ipynb**: A parallel copy of Crypto_Sentiment_Analysis_BERTweet.ipynb where you can find the training of the final versions of the model and the other half for hyperparameter optimization.
4. **Crypto_Relabeling.ipynb**: Contains the process used to generate the new labels specific for Cryptocurrencies.
5. **Model_Evaluation.ipynb**: Code to run the final evaluations of the baseline and optimal model.  

Feel free to connect with me to discuss this project further!
