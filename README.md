# IMDb Movie Reviews: Text Preprocessing for NLP Tasks

### **Description**:
This project focuses on the preprocessing of IMDb movie review data for Natural Language Processing (NLP) tasks. Preprocessing is a critical step before performing advanced NLP tasks like sentiment analysis or classification. This project demonstrates techniques such as cleaning, tokenization, stop word removal, stemming, lemmatization, and visualizing word frequencies before and after preprocessing.

### **Dataset**:
The dataset used in this project consists of 50,000 movie reviews from IMDb (Internet Movie Database), which are labeled as either "positive" or "negative" based on sentiment. The dataset is sourced from [Kaggle](https://www.kaggle.com/datasets/lakshmi25npathi/imdb-dataset-of-50k-movie-reviews).

### Requirements
The following Python libraries are required to run this project:
- Pandas
- NLTK
- BeautifulSoup
- Matplotlib

You can install them using the `requirements.txt` file:
```bash
pip install -r requirements.txt
```

### **Project Workflow**:
1. **Data Cleaning**:
   - Removal of HTML tags and special characters.
   - Removal of punctuation marks.
   
2. **Tokenization**:
   - Breaking down the review text into individual words (tokens).
   
3. **Stop Word Removal**:
   - Filtering out common, non-informative words (e.g., "the", "is") as well as domain-specific words like "movie" and "film".
   
4. **Stemming and Lemmatization**:
   - **Stemming**: Reducing words to their root form (e.g., "running" to "run").
   - **Lemmatization**: Converting words to their dictionary form (e.g., "better" to "good").
   
5. **Word Frequency Visualization**:
   - Visualizing the most common words before and after applying stop word removal.

### **Key Techniques**:
- **Removing HTML Tags**: Cleaned reviews by removing any residual HTML tags such as `<br>`.
- **Tokenization**: Used the NLTK library to tokenize the text, splitting it into individual words.
- **Stop Word Removal**: Utilized NLTK’s built-in stop word list and added custom stop words (like "movie" and "film").
- **Stemming and Lemmatization**: Applied **PorterStemmer** for stemming and **WordNetLemmatizer** for lemmatization to standardize the words.
- **Data Visualization**: Compared word frequencies before and after preprocessing using `matplotlib`.

### **Technologies Used**:
- **Languages**: Python
- **Libraries**: Pandas, NLTK, BeautifulSoup, Matplotlib
- **Dataset**: IMDb Movie Reviews Dataset (sourced from Kaggle)

### **How to Run**:
1. Clone this repository:
   ```bash
   git clone https://github.com/your-username/imdb-text-preprocessing.git
   cd imdb-text-preprocessing
2. Install the required Python libraries:
   ```bash
   pip install -r requirements.txt
3. Run the Jupyter Notebook to view the preprocessing steps and visualizations:
   ```bash
   jupyter notebook

### **Visualizations**:
The project includes bar plots that visualize the most frequent words in the dataset:

- **Before Stop Word Removal**: Words like "the," "and," "movie" dominate the frequency charts.
- **After Stop Word Removal**: More meaningful words such as "good," "bad," and "story" become prominent.

### **Conclusion**:
Effective text preprocessing is vital for extracting meaningful insights from raw text data. In this project, cleaning, tokenizing, and normalizing text (through stemming and lemmatization) significantly improved the quality of the dataset for downstream tasks like sentiment analysis. The visualizations of word frequencies before and after preprocessing highlight how this step refines the dataset.

### **Future Work**:
- Perform sentiment analysis on the preprocessed data.
- Experiment with different stop word lists and preprocessing techniques.
- Explore other NLP tasks such as topic modeling or text classification using machine learning models.

### **License**:
This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.
