# Debiasing Contexual Embeddings
## Project Overview

This project investigates how the Stereotype Content Model (SCM), specifically the dimensions of warmth and competence can be applied to Masked Language Modeling (MLM) for detecting and mitigating bias in profession-related text.

Using a pre-trained BERT transformer model, this study analyzes warmth and competence bias in contextualized word embeddings, evaluates the effectiveness of a projection-based debiasing approach, and assesses the extent to which semantic meaning is preserved after debiasing.

The work addresses context-dependent biases that can affect AI-driven decision-making, particularly in recruitment processes such as candidate shortlisting and screening. The code was developed as part of a Master’s Thesis in Data Science and **the study has been accepted for publication**.

## Technologies
- Python 3.6

- Transformers (BERT)

- NumPy, Pandas, Scikit-learn

- PyTorch/TensorFlow


## Repository Structure 
**data/**  
- Contains all datasets required to run the code  
- Includes `.csv` and `.xlsx` files used in the analysis  

**src/**  
- Code used to generate experimental results  
- Modified model files to ensure reproducibility (relative paths)  
- Profession mapping scripts  
- Exploratory data analysis using NumPy and Pandas on the O*NET data source  


## Results & Conclusion
The results show that SCM-guided projection effectively reduces profession-related stereotype bias in BERT embeddings while preserving semantic meaning.

Across multiple evaluation metrics, the method consistently attenuates warmth and competence stereotypes, remains stable across random seeds and professions, and provides interpretable bias directions grounded in psychological theory. While not eliminating all bias, it offers a lightweight, transparent baseline for multidimensional debiasing.

**Overall, the study demonstrates that psychological models of stereotyping can be operationalized in NLP, enabling practical bias mitigation for high-stakes applications such as recruitment and résumé screening.**


## Running the code
To run the code, install the required dependencies listed in requirements.txt and ensure the data/ directory is present, as the scripts rely on .csv and .xlsx files located there.
