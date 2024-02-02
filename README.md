# From Neurons to Neutrons: A Case Study in Interpretability

Mechanistic Interpretability (MI) promises a path toward fully understanding how neural networks make their predictions. Prior work demonstrates that even when trained to perform simple arithmetic, models can implement a variety of algorithms (sometimes concurrently) depending on initialization and hyperparameters. Does this mean neuron-level interpretability techniques have limited applicability? Here, we argue that high-dimensional neural networks can learn _useful_ low-dimensional representations of the data they were trained on, going beyond simply making good predictions: Such representations can be understood with the MI lens and provide insights that are surprisingly faithful to human-derived domain knowledge. This indicates that such approaches to interpretability can be useful for deriving a new understanding of a problem from models trained to solve it. As a case study, we extract nuclear physics concepts by studying models trained to reproduce nuclear data.

## Getting Started
- Install the requirements using the following command:
```pip install -r requirements.txt```

- Play with the embeddings and last layer features in  ```icml.ipynb```.

## Repository Structure
General file structure, files you may care about:
```
icml.ipynb

src/
  ├── data.py
  ├── model.py
  └── utils.py

data/
  ├── ame2020.csv
  └── ground_states.csv

long-runs/models/
  ├── long_run-binding100+z1+n1+radius0.02+qa200+qbm200+qbm_n200+qec200+sn200+sp200-seed0/
      └── args.yaml
      └── ckpts/
          └── model.pt
```