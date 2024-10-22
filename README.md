# Final Project Report: Hate Speech and the 2022 FIFA World Cup: A Sentiment Analysis Study

**BY:** Abderahman El-Sayyad  
**Supervised by:** Eng. Baraa Abu Sallout

---

## 1. Introduction

The 2022 FIFA World Cup in Qatar was a monumental global event that drew attention to social issues, particularly involving Arab culture and Islam. This project investigates whether public attitudes toward Arabs shifted during and after the World Cup, especially on social media platforms like Twitter. The analysis includes 1 million tweets from December 2022 to November 2022, focusing on detecting changes in sentiment and identifying spikes in hate speech using natural language processing (NLP) techniques.

---

## 2. Problem and Objective

The project seeks to explore whether the 2022 World Cup influenced public sentiment regarding Arabs and Islam. Specifically, it asks:

- Did the public sentiment toward Arabs and Islam change before, during, and after the World Cup?
- Was there an increase in hate speech on these topics?

---

## 3. Dataset Description

### Data Collection

- **Source:** Twitter was scraped for tweets containing keywords such as 'Qatar', 'World Cup', 'Arab culture', and 'Islam'.
- **Sample Size:** 1 million tweets from December 2022 to November 2022.
- **Fields:**
  - Datetime
  - Text
  - Sentiment Label (positive, neutral, negative)
  - Tokenized Text
  - Lemmatized Text
  - Numeric Sentiment Label (0 = negative, 1 = neutral, 2 = positive)

### Preprocessing Steps

1. **Tokenization:** Splitting the text into individual tokens (words or characters).
2. **Lemmatization:** Reducing words to their base form (e.g., 'running' to 'run').
3. **Stopword Removal:** Removing commonly used words that add little meaning (e.g., 'the', 'and').
4. **Special Characters Removal:** URLs, punctuation, and non-alphabetical characters were removed.

---

## 4. Exploratory Data Analysis (EDA)

### 4.1 Sentiment Distribution Before, During, and After the World Cup

The dataset was divided into three time periods:

- **Before:** November 2022 (pre-World Cup).
- **During:** November 20 - December 18, 2022 (World Cup event).
- **After:** Post-December 18, 2022 (post-World Cup).

A count plot visualized the distribution of positive, neutral, and negative tweets across these periods.

![image](https://github.com/user-attachments/assets/4866eb08-696c-4a73-9a48-f8b3b9705f9a)


### 4.2 Tweet Length Distribution

The length of tweets was analyzed to determine whether longer tweets conveyed more emotional or complex content.

- **Observation:** Tweet length increased during the World Cup as people expressed more detailed opinions, and this trend persisted after the event.

![image](https://github.com/user-attachments/assets/d2bc7339-46e2-488f-aa9a-7c7910987313)


### 4.3 Sentiment Over Time

Sentiment was analyzed on a daily basis, with the following key findings:

- A rise in positive sentiment during the World Cup.
- A spike in negative sentiment after specific events related to Arab culture and Islam.

![image](https://github.com/user-attachments/assets/7c6740c2-b898-4356-b0a5-9e2b372ca821)


### 4.4 Word Cloud Analysis

Word clouds visualized the most frequently used words during different periods:

- **Before:** Words like 'Qatar' and 'Islam' were common.
- **During:** Positive words like 'win', 'Arab', and 'historic' were frequent.
- **After:** Negative words related to social issues began to reappear.

![image](https://github.com/user-attachments/assets/8ff9c7fc-d1f8-40d4-bcb9-6cf16e541828)

![image](https://github.com/user-attachments/assets/67410a56-176f-4ac6-8c9a-f6cb483fae0c)

![image](https://github.com/user-attachments/assets/94ec2a0b-a7b1-469d-aedd-fde94a64e7ea)

---

## 5. Sentiment Analysis Model

The `CardiffNLP/twitter-roberta-base-sentiment` model, fine-tuned for Twitter data, was used to classify tweets into Positive, Neutral, and Negative categories. The analysis tracked sentiment changes over time.

---

## 6. Conclusion

The 2022 FIFA World Cup significantly affected public sentiment toward Arabs and Islam on Twitter. There was a noticeable increase in positive sentiment during the World Cup, especially following historic victories by Arab teams. However, negative sentiment rose after the event, especially concerning social and cultural discussions involving Arab culture and Islam.

---

## 7. Future Work

Future research could incorporate more advanced NLP techniques like GPT-4 to better understand the context behind sentiments. Additionally, sentiment analysis could be enhanced by factoring in demographic information to explore regional differences.

---

## 8. References

- (https://huggingface.co/cardiffnlp/twitter-roberta-base-sentiment)

---

