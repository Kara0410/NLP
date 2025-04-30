


          
# Natural Language Processing Project - Document Classification

## Project Overview
This project focuses on implementing document classification models using PyTorch and BERT for natural language processing tasks. The project works with the HumSet dataset, which contains text excerpts from humanitarian response organizations, classified into different humanitarian sectors.

## Dataset
The project uses the HumSet dataset, which includes:
- Training, validation, and test sets in CSV format
- Text excerpts from humanitarian response organizations
- Labels for humanitarian sectors (agriculture, health, protection, etc.)
- Total of 17,301 data points

## Project Structure
The project is divided into two main tasks:

### Task A: Document Classification with PyTorch (25 points)
1. **Data Preprocessing**
   - Loading and cleaning of train, validation, and test datasets
   - Creation of word dictionary
   - Batch processing implementation

2. **Model Architecture**
   - Implementation of `ClassificationAverageModel`
   - Word embedding lookup using pre-trained embeddings
   - Document representation through element-wise mean of word embeddings

3. **Training Pipeline**
   - Loss function: Negative Log Likelihood/Cross Entropy
   - Optimization using Adam
   - Early stopping based on validation accuracy
   - Model evaluation on test set

### Task B: Document Classification with BERT (15 points)
1. **BERT Implementation**
   - Utilization of pre-trained BERT model
   - Fine-tuning for document classification
   - Integration with PyTorch

## Results
The project achieved the following accuracy scores:

For PyTorch Model:
```
Dataset           Accuracy
--------------  ----------
Validation Set    0.568952
Test Set          0.581888
```

## Technical Implementation
- **Libraries Used**: PyTorch, transformers, scikit-learn, numpy, pandas
- **Key Features**:
  - Batch processing with customizable batch size
  - Pre-trained word embeddings
  - Early stopping mechanism
  - Model parameter optimization
  - BERT integration

## Project Setup
1. Install required dependencies:
```bash
pip install torch transformers pandas numpy scikit-learn gensim nltk spacy
```

2. Dataset structure:
```
project/
├── thedeep.subset.train.txt
├── thedeep.subset.validation.txt
├── thedeep.subset.test.txt
├── thedeep.subset.label.txt
└── thedeep.ToU.txt
```

## Contributors
- Boran Cihan Polat (k12005254)
- Halil Atmaca (k12008205)

## Acknowledgments
This project is part of the Natural Language Processing course at Johannes Kepler University (JKU) Linz. The HumSet dataset is provided by the DEEP project (https://www.thedeep.io).

## References
[1] HumSet: Dataset of Multilingual Information Extraction and Classification for Humanitarian Crises Response
*Selim Fekih, Nicolo' Tamagnone, Benjamin Minixhofer, Ranjan Shrestha, Ximena Contla, Ewan Oglethorpe and Navid Rekabsaz.* 
In Findings of the 2022 Conference on Empirical Methods in Natural Language Processing (Findings of EMNLP), December 2022.

        
