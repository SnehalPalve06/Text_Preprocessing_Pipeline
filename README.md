📚 **Text Preprocessing Pipeline using NLP** 
📌 **Project Overview**
This project demonstrates a complete Natural Language Processing (NLP) Text Preprocessing Pipeline. The pipeline collects text data from Wikipedia, cleans and preprocesses the text, converts it into numerical features using TF-IDF, and prepares it for Machine Learning classification tasks.
The objective is to transform raw, unstructured text into a clean and structured format suitable for machine learning models.

🎯 **Objectives**
- Collect text data from Wikipedia
- Perform text cleaning and preprocessing
- Apply NLP techniques
- Convert text into numerical vectors using TF-IDF
- Prepare a dataset for text classification

- **Dataset Categories**
The project collects Wikipedia articles from the following categories:

- Artificial Intelligence
- Climate Change
- Space Exploration
- World History
Each category contains 15 articles.

**Project Workflow**
**Step 1: Data Collection**
wikipedia articles are scraped using:
- Requests
- BeautifulSoup
The main article content is extracted while ignoring references, links, and unnecessary elements.

**Step 2: Text Cleaning**
The following preprocessing operations are performed:
- Remove HTML tags
- Remove citations such as [1], [23]
- Remove punctuation and special characters
- Convert text to lowercase
- Remove extra spaces

**Step 3: NLP Preprocessing**
**Tokenization**
- Text is split into individual words using:  nltk.word_tokenize()

**Stopword Removal**
Common words such as: the, is, and, of, in  are removed.

**Stemming**
Words are reduced to their root forms using: PorterStemmer

**Lemmatization**
- Words are converted to meaningful base forms using: WordNetLemmatizer

**Step 4: Create Final Clean Text**
Processed tokens are joined back into sentences.

**Step 5: TF-IDF Feature Extraction**
- Text is converted into numerical vectors using: TfidfVectorizer
- The dataset is split into:
80% Training Data
20% Testing Data
- TF-IDF helps identify important words in each category.

**Technologies Used**
- Python
- Pandas
- NumPy
- Requests
- BeautifulSoup
- NLTK
- Scikit-Learn

  📁 **Output Files**
**raw_dataset.csv**
- Contains original scraped Wikipedia articles.
**cleaned_dataset.csv**
- Contains cleaned text and tokenized data.
**final_dataset.csv**
Contains:
- clean_text
- Label
- token_count
- clean_token_count
- words_removed
  
📊 **Key Learning Outcomes**
- Web Scraping using BeautifulSoup
- Text Cleaning Techniques
- Tokenization
- Stopword Removal
- Stemming and Lemmatization
- TF-IDF Vectorization

**Future Improvements**
- Train Machine Learning classifiers
- Compare TF-IDF with Word2Vec and BERT embeddings
- Perform Text Classification
- Add Data Visualization
- Build a complete NLP prediction system
- NLP Data Preparation Pipeline
  
🚀 Future Improvements
Train Machine Learning classifiers
Compare TF-IDF with Word2Vec and BERT embeddings
Perform Text Classification
Add Data Visualization
Build a complete NLP prediction system

👨‍💻 **Author**
  Snehal Palve
**Email**
snehalpalve02@gmail.com
