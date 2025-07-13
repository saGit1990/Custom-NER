# 📦 Named Entity Recognition with spaCy 

This project demonstrate how to train a custom Named Entity Recognition (NER) model

----
## **Objective**
- Train a custom NER model to identify entities such as:
 - Organization (ORG)
 - Medicine (medicine)
 - Persons (PERSON)
 - Monetary values (MONEY)
 - Dates (DATE)

----
## 📁 **Dataset**
- Downloaded the dataset from Kaggle Medicle NER dataset. (https://www.kaggle.com/datasets/finalepoch/medical-ner)
- Stored in spaCy's 'DocBin'

----
## 🧪 **Tools & Framework**
- spaCy 
- DocBin for efficient binary training format
- spaCy train for model training

----
## **Project Structure**
- ner-day5/
    - train.spacy # Annotated training data 
    - config.cfg # spaCy training configuration
    - best_config.cfg 
    - custom-NER.ipynb # training script
    - README.md 
    - requirements.txt

----
## **Sample input & Output**
Input:
    While bismuth compounds (Pepto-Bismol) decreased the number of bowel movements in those with travelers' diarrhea, they do not decrease the length of illness.[91] Anti-motility agents like loperamide are also effective at reducing the number of stools but not the duration of disease.[8] These agents should be used only if bloody diarrhea is not present.

Predicted Entities:
 - bismuth compounds  ->  medicine
 - Pepto-Bismol       ->  medicine
 - diarrhea           ->  medicalcondition

----

## 📈**Future Work**
- Expand dataset with more custom entity types
- Evaluate with Precision / Recall / F1
- Deploy as a REST API
- Compare spaCy with HuggingFace NER Models

----

## **Key Learning**
Using spaCy DOCBIN format makes it easy to annotate and train custom NER models - even with small datasets. This form a strong foundation for domain-specific NER (legal, medical, finance, etc.).

**Part of my 24-Day NLP Spring Day#5**