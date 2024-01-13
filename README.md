# Sample Code for Classifying Manifestos into Topics
**Author:** Guillermo Lezama

## Overview
This repository contains the code used in my dissertation paper's analysis. The objective is to identify the issues discussed in politicians' proposals by analyzing 11,422 mayoral candidates' manifestos from Brazil's 2012 election.

## Contact
For questions, suggestions, or comments, please email: guillelezama@pitt.edu

## Methodology
1. **Data Collection**: Scraped PDFs of manifestos from the TSE website using candidate IDs, converting them into JSON format.
2. **Pre-processing**: Cleaned and compiled JSONs into a dataframe.
3. **Manual Coding**: Coded 100 manifestos into 10 topics manually.

## Workflow
1. Load necessary packages.
2. Implement data cleaning programs.
3. Load and process data; split into train and test sets.
4. Run and evaluate four different model sets.
5. Select the best model.
6. Apply model to predict topics for each line in the entire corpus.
7. Present descriptive statistics.

## Inputs
- Stop words lists.
- Manually classified manifestos (`lineas_id1.csv` and `lineas_id2.csv`).
- Full corpus with candidate IDs (`lineas_id_tot.csv`).

## Outputs
- Classified lines with probabilistic topic assignments (`topic_probs.csv`).

## Additional Resources
See `\Examples` for PDF and JSON examples of manifestos.
