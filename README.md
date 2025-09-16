# Spam-Detection - Natural Language Processing Project
This project implements a binary text classification system to distinguish between spam and legitimate messages, addressing real-world challenges in automated email and message filtering.


<img width="648" height="300" alt="image" src="https://github.com/user-attachments/assets/794c7982-c462-48b0-a868-61a0bfe6b05e" />


## Training Data
This contains a CSV file with 3619 labeled samples, of which 1068 are classified as 'spam' and 2551 as 'not-spam'. This dataset size is sufficient to train a machine learning model capable of learning the distinguishing features between legitimate and spam messages.

## Test Data
This contains a CSV file with 1552 unlabelled samples. The model is required to perform inference on this dataset and accurately classify each sample as either 'spam' or 'not-spam'.

## Results 
The python notebook generates a CSV file with predictions on the unlabelled dataset and stores it in your working directory.

```
├── Results
│   ├── results_task1.csv
├── Training and Test Data
│   └── spam_detection_training_data.csv
│   └── spam_detection_test_data.csv
├── Spam_Detection_Task1.ipynb
└── README.md
```

### Procedure 
* Comprehensive text preprocessing including lowercasing, removal of punctuation/special characters, tokenisation, stopword removal, and stemming to normalise and clean the dataset.
* Engineered TF-IDF vectorisation with both unigrams and bigrams, capped at the top 5,000 most frequent terms to balance contextual richness with computational efficiency.
* Trained and evaluated Multinomial Naïve Bayes and Logistic Regression classifiers, analysing trade-offs between speed, interpretability, and predictive performance.

<img width="824" height="351" alt="image" src="https://github.com/user-attachments/assets/63bc3aee-3695-4c42-a649-7421a98bde0b" />


### Accuracy
Achieved 96% accuracy with Naïve Bayes and 98% accuracy with Logistic Regression on the validation set, with the latter demonstrating superior precision, recall, and F1-scores.

	Precision	Recall	F1-score	Support
Not Spam (0)	0.99	0.94	0.96	509
Spam (1)	0.88	0.97	0.92	215
				
Accuracy			0.95	724
Macro Avg	0.93	0.96	0.94	724
Weighted Avg	0.95	0.95	0.95	724
<img width="521" height="169" alt="image" src="https://github.com/user-attachments/assets/bbb642f5-4484-402c-a606-522d2b5eefb5" />


