# **NERandClassification**

Named entity recognition and Sequence classification with Vietnamese


# **Contents**
- [Overview](#overview)
- [Installation](#installation)
- [Settings](#settings)
- [Dataset](#dataset)
- [Training](#training)
- [Evaluate](#evaluate)

# **Overview**
A project to recognize 3 named entiny (product , phone, address) and classify customer intents in Vietnamese message

# **Installation**

## *Create environment*

1. Install miniconda or anaconda.
2. Create conda environment

    ```bash
    conda create -n NERC python=3.9.5
    conda activate NERC
    ```


## *Install dependencies*

1. Important Dependencies
    ```bash
    pip install -r requirements.txt
    ```

# **Settings**
Load arguments in TrainingArguments from Transformer library
    
    from transformers import TrainingArguments, Trainer
    training_args = TrainingArguments("test-trainer",remove_unused_columns = False, num_train_epochs=5, logging_steps=200per_device_train_batch_size=4,evaluation_strategy="steps", eval_steps=200)

# **Dataset**
    Dataset of 5000+ message from Vietnamese customer 
## *Downloading data*
    Dataset can be download at [Driver](https://docs.google.com/spreadsheets/d/1iiaUl1mmY9vZFNGjfaXxSmIb0aSfOLmv/edit?usp=drive_link&ouid=107321072786087136500&rtpof=true&sd=true)

## *Create training & testing dataset*
    run file multifr.ipynb

# **Training**
    run file multifr.ipynb

# **Evaluate**

![Screenshot 2024-05-22 001454](https://github.com/duysop/NERandClassification/assets/103120531/7de446d1-b40a-41e3-a470-a8243a675c17)
