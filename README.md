# TEXT-SUMMARIZATION-TOOL

*COMPANY* : CODTECH IT SOLUTIONS

*NAME* : KUMILI VINESH

*INTERN ID* : CITSOD647

*DOMAIN* : ARTIFICIAL INTELLIGENCE

*DURATION* : 4 WEEKS

*MENTOR* : NEELA SANTOSH

 This project focuses on extractive text summarization using the TextRank algorithm, implemented in Python within the Google Colab environment. The goal of the task is to automatically generate concise summaries from longer text documents by identifying and extracting the most important sentences. Extractive summarization differs from abstractive summarization in that it selects sentences directly from the original text instead of generating new content. The core of the method relies on computing the similarity between sentences and building a graph where each node represents a sentence, and edges represent how similar those sentences are. The more a sentence resembles other sentences, the more central or "important" it is considered. The ranking of sentences is achieved using the PageRank algorithm, originally designed for ranking web pages.

The project makes use of several key Python libraries. The Natural Language Toolkit (NLTK) is used for basic natural language processing tasks such as removing stopwords, which are common words like “the,” “and,” or “is” that do not contribute significant meaning in similarity calculations. NumPy is used for handling numerical operations and to build the sentence similarity matrix. NetworkX, a library for network analysis, is used to construct the graph of sentences and to apply the PageRank algorithm that scores sentence importance. Additional support is provided by Python’s built-in re module to clean text using regular expressions. The development environment for this project is Google Colab, a powerful and accessible cloud-based platform that allows users to write and run Python code without needing to install anything locally. Colab supports direct file uploads, inline execution, and easy library installation, making it ideal for rapid development and experimentation in natural language processing projects like this one.

The summarization process follows a clear workflow. First, the input text is read from a .txt file and preprocessed: it is split into sentences, cleaned of non-alphabetical characters, and tokenized into words. Stopwords are removed from these tokens to reduce noise. Next, each sentence is compared to every other sentence using cosine similarity, resulting in a similarity matrix that quantifies how closely related each pair of sentences is. This matrix is then used to construct a graph, where sentences are nodes and edges are the similarity values. The PageRank algorithm is applied to score each sentence based on its connectivity and importance within the graph. Finally, the top-ranked sentences are selected and joined to form the summary. The number of sentences in the summary can be customized through a parameter in the function.

This summarization method is applicable across many domains. In journalism, it can help readers quickly understand lengthy articles by presenting only the most relevant sentences. In education, it can assist students in studying by summarizing textbooks or lecture transcripts. In legal and medical fields, it can extract critical points from long and complex documents. Businesses can use summarization tools to condense meeting minutes, reports, or emails, increasing productivity. Additionally, this technology can be integrated into chatbots or virtual assistants to provide brief and informative responses. Despite its simplicity, the model has some limitations. For example, using a basic method to split sentences based on periods (.split(". ")) can lead to errors, especially with abbreviations. Also, using plain word matching for similarity ignores the deeper semantic meaning that modern techniques like word embeddings or transformer-based models can capture.

In conclusion, this extractive text summarizer demonstrates how traditional NLP techniques—when combined with graph theory and mathematical tools—can effectively summarize large volumes of text. The implementation in Google Colab allows for easy accessibility and testing, making it an ideal learning project for understanding the fundamentals of natural language processing and text summarization.

*OUTPUT*
https://github.com/user-attachments/assets/6328f07d-631e-4473-b345-121ac509b52b
