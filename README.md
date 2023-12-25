# Text-Similarity-with-SpaCy
Measure text similarity using SpaCy's similarity function.
import spacy

nlp = spacy.load('en_core_web_sm')

text1 = "Natural language processing is a subfield of artificial intelligence."
text2 = "NLP is a branch of AI that deals with the interaction between computers and humans using natural language."

doc1 = nlp(text1)
doc2 = nlp(text2)

similarity = doc1.similarity(doc2)
print(f"Text Similarity: {similarity}")
