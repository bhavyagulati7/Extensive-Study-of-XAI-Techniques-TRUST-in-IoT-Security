# Extensive Study of XAI Techniques: LIME, SHAP & TRUST for IoT Security

**Authors:** Parul Gupta, Bhavya Gulati, Gaurav Singal, Riti Kushwaha, Ashish Sharma  
*This repository* contains the code and notebooks used in the manuscript *“An Extensive Study of XAI Techniques LIME, SHAP, TRUST in IoT Security”*.

## Abstract

As Internet of Things (IoT) deployments continue to expand, network intrusion detection systems (IDS) must not only achieve high accuracy but also provide transparency to their users.  
This work presents a **systematic, side-by-side comparison** of three Explainable AI (XAI) techniques — **LIME**, **SHAP**, and the recently proposed **TRUST XAI** — applied to a common neural network–based IDS trained on two heterogeneous IoT traffic datasets: **NSL-KDD** and **TON-IoT**.  

We evaluate each method across multiple dimensions, including:
- **Local and global interpretability**
- **Fidelity of explanations**
- **Computational cost**
- **Stability under input perturbations**

Our experiments reveal that no single explainer dominates across all conditions:
- **SHAP** provides the most consistent global insights on balanced, low-dimensional data (e.g., NSL-KDD).  
- **LIME** excels at generating rapid, instance-specific explanations in moderately complex environments (e.g., TON-IoT).  
- **TRUST XAI** combines probabilistic interpretability with low runtime overhead, making it particularly well-suited for large-scale, high-dimensional IoT scenarios.  

Finally, we distill these findings into **practical guidelines** for selecting the most suitable XAI approach based on performance needs, dataset complexity, and runtime constraints. This study aims to advance both the **transparency** and **trustworthiness** of AI-driven IoT security solutions.




## Setup and Execution

### 1. Upload the Datasets
You can download the datasets from:
- **NSL-KDD:** [https://ieee-dataport.org/documents/nsl-kdd](https://ieee-dataport.org/documents/nsl-kdd)
- **TON-IoT:** [https://research.unsw.edu.au/projects/toniot-datasets](https://research.unsw.edu.au/projects/toniot-datasets)

Upload the dataset files (e.g., `KDDTrain+.txt`, `KDDTest+.txt`, `Train_Test_Network.csv`, etc.) to your Google Drive or the Colab environment.

### 2. Open the Colab Notebooks
Choose the notebook corresponding to your dataset
### 3. Update Dataset Paths
In the first few cells of the notebook, update the dataset path:
```python
data_path = "/content/drive/MyDrive/NSL_KDD/KDDTrain+.txt"  # Example for NSL-KDD

