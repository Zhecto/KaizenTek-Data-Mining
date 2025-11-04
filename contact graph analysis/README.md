# Contact Graph Analysis

A comprehensive network analysis of contact tracing data to identify patterns, communities, and key individuals in social contact networks.

## Overview

This project analyzes contact tracing datasets to understand interaction patterns, identify superspreaders, detect community structures, and predict potential future contacts.

## Project Structure

```
contact graph analysis/
├── KaizenTek.ipynb          # Main analysis notebook
├── notebooks/               # Individual analysis notebooks
│   ├── centrality_analysis.ipynb
│   ├── community_detection.ipynb
│   ├── data_exploration.ipynb
│   ├── LinkPrediction.ipynb
│   ├── data_preprocessing.ipynb
│   └── datasets/            # Processed datasets
└── requirements.txt         # Python dependencies
```

## Analysis Components

1. **Data Preprocessing** - Clean and merge contact tracing datasets
2. **Data Exploration** - Statistical analysis and visualization of contact patterns
3. **Network Visualization** - Temporal network graph construction
4. **Centrality Analysis** - Identify key individuals and superspreaders
5. **Community Detection** - Detect social clusters using Louvain algorithm
6. **Link Prediction** - Predict potential future contacts using ML

## Requirements

- Python 3.8+
- NetworkX 3.1
- pandas, numpy, matplotlib, seaborn
- scikit-learn
- python-louvain
- node2vec

Install dependencies:
```bash
pip install -r requirements.txt
```

## Usage

1. Place contact tracing `.dat` files in `datasets/source_datasets/`
2. Run `KaizenTek.ipynb` or individual notebooks in `notebooks/`
3. Processed data will be saved to `datasets/compiled_merged_dataset/`

## Dataset Format

Input files should be space-delimited with format:
```
timestamp person_A person_B
```

Metadata files (optional):
```
person_id group_label
```

## Key Findings

- Degree distribution analysis reveals contact frequency patterns
- Group homophily shows intra-group vs inter-group contact preferences
- Temporal patterns identify peak contact hours
- Community detection reveals natural social clusters
- Link prediction achieves high accuracy using Node2Vec embeddings

## License

MIT
