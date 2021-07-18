# News_Headline_Classification

## Classification with BERT

### 1. binary classification: >=9%

- Baseline model

| | precision  | recall | f1-score | support | 
| ------------- | ------------- | ------------- | ------------- | ------------- |
| other  | 0.87  | 0.95 | 0.91 | 2477 |
| >=9%  | 0.30  | 0.13 | 0.18 | 412 | 


| | Predict other  | Predict >=9% | 
| ------------- | ------------- | ------------- | 
| True other  | 2348  | 129 | 
| True >=9%  | 357 | 55 | 

- Data augmentation

| | precision  | recall | f1-score | support | 
| ------------- | ------------- | ------------- | ------------- | ------------- |
| other  | 0.87  | 0.92 | 0.90 | 2477 |
| >=9%  | 0.27  | 0.17 | 0.21 | 412 | 


| | Predict other  | Predict >=9% | 
| ------------- | ------------- | ------------- | 
| True other  | 2290  | 187 | 
| True >=9%  | 343 | 69 | 

### 2. binary classification: <=-9%

- Baseline model

| | precision  | recall | f1-score | support | 
| ------------- | ------------- | ------------- | ------------- | ------------- |
| other  | 0.90 | 1.00 | 0.95 | 2588 |
| <=-9%  | 0.00  | 0.00 | 0.18 | 301 | 


| | Predict other  | Predict >=9% | 
| ------------- | ------------- | ------------- | 
| True other  | 2588  | 0 | 
| True <=-9%  | 301 | 0 | 

- Data augmentation

| | precision  | recall | f1-score | support | 
| ------------- | ------------- | ------------- | ------------- | ------------- |
| other  | 0.90 | 0.93 | 0.92 | 2588 |
| <=-9%  | 0.17  | 0.12 | 0.14 | 301 | 


| | Predict other  | Predict >=9% | 
| ------------- | ------------- | ------------- | 
| True other  | 2408  | 180 | 
| True <=-9%  | 265 | 36 | 


### 3. 3 class classification

- Baseline model

| | precision  | recall | f1-score | support | 
| ------------- | ------------- | ------------- | ------------- | ------------- |
| <=-9%  | 0.45  | 0.02 | 0.03 | 301 | 
| other  | 0.76 | 1.00 | 0.83 | 2176 |
| >=9%  | 0.39  | 0.02 | 0.04 | 412 | 


| | Predict <=-9% | Predict other  | Predict >=9% | 
| ------------- | ------------- | ------------- | ------------- | 
| True <=-9%  | 5 | 290 | 6 | 
| True other  | 2 | 2166  | 8 | 
| True >=9%  | 4 | 399 | 9 | 

- Data augmentation

| | precision  | recall | f1-score | support | 
| ------------- | ------------- | ------------- | ------------- | ------------- |
| <=-9%  | 1.00  | 0.00 | 0.01 | 327 | 
| other  | 0.75 | 0.98 | 0.85 | 2398 |
| >=9%  | 0.24 | 0.16 | 0.19 | 412 | 


| | Predict <=-9% | Predict other  | Predict >=9% | 
| ------------- | ------------- | ------------- | ------------- | 
| True <=-9%  | 51 | 214 | 36 | 
| True other  | 174 | 1825  | 177 | 
| True >=9%  | 43 | 303 | 66 | 


## Classification with Snorkel

| | precision  | recall | f1-score | support | 
| ------------- | ------------- | ------------- | ------------- | ------------- |
| <=-9%  | 0.19  | 0.17 | 0.18 | 301 | 
| other  | 0.78 | 0.84 | 0.81 | 2176 |
| >=9%  | 0.21 | 0.02 | 0.04 | 412 | 


| | Predict <=-9% | Predict other  | Predict >=9% | 
| ------------- | ------------- | ------------- | ------------- | 
| True <=-9%  | 1 | 325 | 1 | 
| True other  | 0 | 2357  | 41 | 
| True >=9%  | 0 | 442 | 11 | 

