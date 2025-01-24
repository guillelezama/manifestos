# Exploring the Impact of Corruption on Political Proposals: A Text Classification Problem
**Author:** Guillermo Lezama

## Overview
This repository shows the methodological framework I developed for one chapter of my dissertation, where I explored how corruption scandals influence politicians' rhetoric and policy priorities. Specifically, the research investigates whether a high incidence of corruption in a particular area, such as health, drives politicians to either increase or decrease their focus on that topic in their campaign proposals.

To address this question, I analyzed a dataset of over 13,000 campaign manifestos from mayoral elections in Brazil. Each manifesto was broken down into sentences, creating a corpus for classification. As a resource-constrained graduate student, I manually classified approximately 1% of the dataset to generate labeled training data. In practice, scaling this task would ideally involve research assistants, but this exercise showcases the creative solutions I employed within limited resources.

Through this project, I demonstrate my ability to handle unstructured text data, apply machine learning models, and leverage external APIs to enhance analysis. This notebook is not just an extension of my dissertation—it’s a showcase of my technical skills, and commitment to addressing complex research questions with innovative approaches.

In the notebook classification_openai.ipynb, I pre-process the data, define the test-train split, and train the ML models.

In the notebook classification_openai.ipynb, I incorporate OpenAI's API as a benchmark for text classification results.

In the notebook classification_analysis.ipynb, I analyze all the results.

Link to the paper: https://guillelezama.netlify.app/uploads/jmp.pdf

## Contact
For questions, suggestions, or comments, please email: guillermo.lezama [at] pitt [dot] edu

## Methodology
1. **Data Collection**: Scraped PDFs of manifestos from the TSE website using candidate IDs, converting them into JSON format.
2. **Pre-processing**: Cleaned and compiled JSONs into a dataframe.
3. **Manual Coding**: Coded 100 manifestos into 10 topics manually.

## Workflow
This project involves a multi-step workflow to classify text data and analyze the results:


1. Load necessary packages.
2. Implement data cleaning programs.
3. Load and process data; split into train and test sets.
4. Run and evaluate four different model sets.
5. Select the best model.
6. Apply model to predict topics for each line in the entire corpus.
7. Present descriptive statistics.

## Workflow
- classification_ML.ipynb: This notebook handles data preprocessing, defines the train-test split, and trains multiple machine learning models. Additionally, it trains different ML models (NB, SVC, RF, KN, LSTM).

- classification_openai.ipynb: It integrates OpenAI's API as a benchmark for text classification results.

- classification_analysis.ipynb: This notebook focuses on analyzing and comparing the classification results, presenting insights through descriptive statistics and visualizations.

## Inputs
- Stop words lists.
- Manually classified manifestos (`sample_lines.csv`).

## Outputs
- Test data (`test_data_for_openAI.csv`).
- Classified lines with topic assignments using ML (`predictions.csv`).
- Classified lines with topic assignments using OpenAI (`test_data_for_openAI_predictions.csv`).

# Additional Resources
- See \Examples for PDF and JSON examples of manifestos.
- slides_text_classification.pdf summarizes the project
