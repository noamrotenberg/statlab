
# statlab
[![PyPi version](https://badgen.net/pypi/v/statlab)](https://pypi.org/project/statlab)

statlab is a new Python package offering a variety of statistical and machine learning tools.


# Products

## "ord" ordinal classification tools
Submodule contains:
+ TreeOrdinalClassifier
+ DifferenceOrdinalClassifier
+ Functions to calculate classification metrics on ordinal data

Methods details and cite: Rotenberg, N. H., Faria, A. V., & Caffo, B. (2026). Classifier Pooling for Modern Ordinal Classification. arXiv preprint [arXiv:2603.17278](https://arxiv.org/pdf/2603.17278).

Submodule developed by: Noam Rotenberg, Andreia Faria, Brian Caffo

Example available in examples/ord.ipynb

## "aled" Adaptive Label Error Detection
Submodule contains: ALEDDetector class

Methods details and cite: Chaudhry, Z., Rotenberg, N. H., Caffo, B., Jones, C. K., & Sair, H. I. (2026). Adaptive Label Error Detection: A Bayesian Approach to Mislabeled Data Detection. arXiv preprint [arXiv:2601.10084](https://arxiv.org/pdf/2601.10084).

Submodule developed by: Zan Chaudhry, Noam Rotenberg, Brian Caffo, Craig Jones, Haris Sair

Example available in examples/aled-medMNIST.py

# Usage

Install: ``!pip install statlab``

Import a single module: ``import statlab.ord`` - imports only ord

Import all modules: ``from statlab.all import *`` - can access any function without prefixes, e.g., ``TreeOrdinalClassifier(base_clf)``

Specific example:
```
!pip install statlab
import statlab.ord
base_clf = # some sklearn-style classifier
clf = statlab.ord.TreeOrdinalClassifier(base_clf)
```

# Future work:

+ Naive Bayes classifier using nonparametric statistics
+ Automated nonlinear feature tuning
