# PySyft for Personalized Federated Advertising


## Summary
Implementation of several Personalized Federated Learning (PFL) and Federated Learning (FL) architectures via PySyft. This was done for my Master's Thesis. 

## Findings

- Implementations of FL and PFL through model aggregation and passing of model dictionaries through PySyft
- Description and analysis of performance metrics of FL and PFL architecture
- Discussion of results and (dis)advantages of implemented architectures

## Results
The following are uploaded as CSV files in the Results folder

- Metrics of implementations 
- Summary metrics

## Thesis

The thesis document, including thorough analysis, summaries, and discussion will be uploaded here once finished.

## Notebooks

The notebooks folder contains all Jupyter Notebooks used. 

### Datasets
The dataset linked under sources needs to be downloaded to replicate the results locally. Both the full dataset (Full) and a randomly sampled 10% (10%) version were used.

### Dataset Modifications
Each dataset has three variants:
- Regular (unchanged)
- Faktor 2 (where the first data selice's numerical values are multiplied by 2, the second's are divided by 2  )
- Random Noise (where random noise was added to the first data slice, and the second reamins the same)

### Architectures
Each dataset modification has four variants. Each notebooks represetns one such variant.
- Central (Non-Federated)
- FedAvg (FL)
- APFL (A version of PFL)
- FedPer (Another version of PFL)



## Sources

### The Dataset
The dataset used was originally provided by Criteo for the <a href="https://www.kaggle.com/competitions/criteo-display-ad-challenge">Criteo Display Advertising Challenge</a>.
The data was accessed <a href="https://tianchi.aliyun.com/dataset/144733">here</a>.<br />

### The Original Model
The DLRM model used for this implementation was based <a href="https://www.kaggle.com/code/egordm/deep-learning-recommendation-model-dlrm">this public Kaggle Submission for the challenge</a>. The submission is an implementation of [this paper ](https://arxiv.org/abs/1906.00091)in Tensorflow.

### Federated Architectures
All Implementations are simplified versions of published Federated Learning achritectures:

</td>
<td valign="top">

- [Federated Averaging (FedAvg)](https://arxiv.org/abs/1602.05629)</a>
- [Adaptive Personalized Federated Learning (APFL)](https://arxiv.org/abs/2003.13461)</a>
- [Federated Personalization (FedPer)](https://arxiv.org/pdf/1912.00818.pdf)</a>

</td>

### PySyft

Syft 0.8.4 was used. For the documentation and installation, refer to the [this document](https://openmined.github.io/PySyft/) and the [PySyft GitHub community](https://github.com/OpenMined/PySyft).
