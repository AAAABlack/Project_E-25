# Project E-25
# Overview

This notebook supports the final report for Project E-25, focusing on analysis and supervised learning applied to network traffic data for intrusion detection systems. It demonstrates a realistic, packet-level IDS flow rather than a time based log analysis.

# Objective

The goal is to evaluate whether statistical features observed from individual packets can be used to determin benign from malicious traffic under practical constraints.

# Data Sources:

- Incribo cybersecurity attack dataset (Kaggle)

- Multiple merged CIC-IDS 2017 dataset (UNB)

- Official IANA service CSV (IANA)

Each packet is treated as an independent observation, reflecting how many IDS systems operate.

# Notebook Structure

Data Loading & Cleaning: normalization, missing value checks, label inspection, duplicate checks.

Feature Enrichment: Port to service mapping, protocol parsing, traffic statistics.

Exploratory Analysis: Class imbalance inspection, feature distributions, correlation checks.

Modeling: Multiple supervised classifiers trained on enriched packet level features.

Evaluation: Precision, recall, F1-score, k-fold cross validations, and confusion matrices with emphasis on false negatives.

# Key Notes & Limitations

- Severe class imbalance is present and explicitly mentioned.

- Results are exploratory, not production ready yet. 

- Temporal correlations between packets are intentionally ignored to mimic stateless IDS behavior.

# Outputs

- Feature distribution plots, both static and browser rendered. 

- Model performance metrics.

- Comparative evaluations 
 
# Important!

If there are any issues with your GIT LFG, please consider directly downloading the datatsets from the sources at the very top of the notebook. 