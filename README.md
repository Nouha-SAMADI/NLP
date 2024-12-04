# NLP-Lab: Deep Learning for Arabic Text Classification  

This lab focuses on exploring natural language processing (NLP) techniques and leveraging deep learning models to classify Arabic text data.

---

## Objective  
The main objective of this lab is to build, train, and evaluate language models for classifying Arabic text data related to a specific topic, with an emphasis on applying advanced sequence models.

---

## Part 1: Classification Task  

### Data Collection  
Arabic text data was collected using [Webteb](https://www.webteb.com/neurology/diseases), a website that provides medical information. Python web scraping libraries such as `BeautifulSoup` and `Scrapy` were used to extract textual data from the neurology section.

### Text Scoring  
To quantify the relevance of each text, a scoring mechanism was implemented. Each text was assigned a score between **0 and 10** based on its alignment with the chosen topic. The score reflects the relevance of the content to the specific field (e.g., neurology) and the presence of key terms.

### Preprocessing Pipeline  
The collected dataset underwent extensive preprocessing to prepare it for training:
1. **Tokenization**: Splitting text into words or phrases.
2. **Stemming & Lemmatization**: Reducing words to their base or dictionary forms.
3. **Stop Word Removal**: Removing common but irrelevant words.
4. **Discretization**: Optional conversion of scores into categories if necessary.

### Model Training  
Four recurrent neural network architectures were implemented to train the classification models:
1. **RNN (Recurrent Neural Network)**
2. **Bidirectional RNN**
3. **GRU (Gated Recurrent Unit)**
4. **LSTM (Long Short-Term Memory)**

Hyperparameter tuning was performed to improve model performance, focusing on parameters such as learning rate, batch size, and sequence length.

### Model Evaluation  
The trained models were evaluated using a combination of standard and NLP-specific metrics:
- **Standard Metrics**: Loss, Accuracy, Precision, Recall, F1-score.
- **NLP-Specific Metrics**: BLEU score, assessing the quality of the text relevance classification.

### Conclusion  
The evaluation results highlighted that the **GRU** model provided a balance between performance and computational efficiency. Further refinement, including advanced preprocessing and hyperparameter tuning, could enhance performance.  

This lab showcases the applicability of deep learning techniques to Arabic text classification and provides a foundation for more complex NLP tasks in the future.
