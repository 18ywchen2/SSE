# SSE

Cross-Project Defect Prediction via Semantic and Syntactic Encoding

## About

Cross-Project Defect Prediction (CPDP) is a promising research field that focuses on detecting defects in projects with limited labeled data by utilizing prediction models trained on projects with abundant data. However, previous CPDP approaches based on Abstract Syntax Tree (AST) have often encountered challenges in effectively acquiring semantic and syntactic information, resulting in their limited ability to combine both productively. This issue arises primarily from the practice of flattening the AST into a linear sequence in many AST-based methods, leading to the loss of hierarchical syntactic structure and structural information within the code. Besides, other AST-based methods use a recursive way to traverse the tree-structured AST, which is susceptible to gradient vanishing. To alleviate these concerns, we introduce a novel CPDP method named defect prediction via Semantic and Syntactic Encoding (SSE) that enhances Zhang's approach by encoding semantic and syntactic information while retaining and considering AST structure. Specifically, we perform pre-training on a large corpus using a language model to learn semantic information. Next, we present a new rule for splitting AST into subtrees to avoid vanishing gradients. Then, the absolute paths originating from the root node and leading to the leaf nodes are encoded as hierarchical syntactic information. Finally, we design an encoder to integrate syntactic information into semantic information and leverage Bi-directional Long-Short Term Memory to learn the entire tree representation for prediction.

## Requirements

SSE is executed on Linux (ideally Ubuntu 22.04.3).

## Prerequisites & Installation

* pip

    In your virtual environment, run:

    ```sh
    pip install -r requirements.txt
    ```

    to install the required packages.

## Quick Start

preprocessing
```
python preprocessing.py
```

running
```
python run.py
```

## 
More details and code comments are being added!
