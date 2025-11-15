# Susmitha-Home-work-4-ML
Name: Susmitha Dodla
ID: 700765311

⸻

Q1: Text Processing Pipeline (nlp_pipeline.py)

In this Python script, I used spaCy to build a simple NLP pipeline that cleans and processes text. The steps are straightforward:
	•	First, the text gets tokenized into individual words.
	•	Then I remove stopwords and punctuation so that only the meaningful words stay.
	•	After that, I apply POS tagging and keep only nouns and verbs using the universal POS tags.
	•	Finally, I lemmatize the remaining words so everything is in its base form (ex: enjoys → enjoy, reading → read).

Input:
“John enjoys playing football while Mary loves reading books in the library.”

Expected Output:
['John', 'enjoy', 'play', 'football', 'Mary', 'love', 'read', 'book', 'library']

⸻

Q2: NER and Ambiguity Check (ner_and_ambiguity.py)

This script does two things:
	•	It extracts named entities like people, locations, and organizations using spaCy’s NER.
	•	It also checks for possible pronoun ambiguity by looking for “he”, “she”, or “they”. If these appear when multiple people are mentioned, it may be unclear who the pronoun refers to.

Input:
“Chris met Alex at Apple headquarters in California. He told him about the new iPhone launch.”

Since the sentence contains “He”, the script correctly prints:
Warning: Possible pronoun ambiguity detected!
