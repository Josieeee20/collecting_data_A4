# collecting_data_A4
This repository is only for assignment
# Corpus Documentation

## 1. The Corpus Itself

This corpus mainly collects the Wikipedia information of the Korean boy group 'NCT_127' 'NCT_dream' 'WAYV'.

## 2. Target Audience and Intended Use

The target audience for this corpus includes fans of the respective groups and enthusiasts of Korean pop culture, aiming to help them understand the positioning and development of the three groups. This contribution is valuable for research in the field of Korean pop culture.

## 3. Text Selection Criteria

The selection criteria focus on text files in the TXT format, primarily related to the specific musical group. Documents are downloaded from Wikipedia to ensure relevance to the chosen musical ensemble.

## 4. Data Collection Process

Utilizing the functionalities of `spacy`, `os`, `csv`, `BeautifulSoup`, and `requests` for data retrieval.

## 5. Cleaning and Preprocessing Steps

Performed initial cleaning on the collected documents, which involved tasks such as removing whitespace, standardizing text format, handling missing data, and addressing case sensitivity.

## 6. Annotations and Tools

we use spacy to annotate the text: coarse-grained tagging, which predicts the simple universal part-of-speech of each token (e.g., noun, verb), and detailed tagging, which uses a more fine-grained set of part-of-speech tags (e.g., 3rd person singular present verb). The tags are determined by the English language model used, and the example mentions the usage of the small English model.

To extract part-of-speech tags, the text suggests creating a function that can extract both coarse- and fine-grained part-of-speech for each token in a spaCy Doc object. The function is expected to utilize token.pos_ for coarse-grained tagging and token.tag_ for fine-grained tagging. The recommendation is to apply this function to each Doc object in a DataFrame containing text data.

## 7. Format of Files in the Corpus
we firstly use txt format to collect all the text then use csv format to analysis it.
| Column            | Description                                                                                       |
|-------------------|---------------------------------------------------------------------------------------------------|
| Filename      | The name of the original text file in the data folder, serving as a unique identifier for each document.                                        |
| Title  | Column containing titles associated with the texts, providing additional context or information about the content of each document.  |
| Doc            | Stores the original text exactly as it appears in the text file, preserving the raw, unprocessed content of each document.                             |
| Text  |  Column containing preprocessed text of each document, including cleaned or modified versions of the original text.                      |
| Tokens         | Stores the tokenized text of each document, representing individual units such as words or punctuation after tokenization.                           |
| Lemmas         | Stores the lemmatized text of each document, containing base or dictionary forms of words obtained through lemmatization.                            |
| Parts-of-speech | Contains information about the parts of speech of all the tokens in each document, including either coarse-grained (universal) or fine-grained part-of-speech tags. |



