Arabic Disease Text Classification Pipeline: A Report
This report details the development of a web scraping and NLP pipeline for Arabic disease classification, focusing on data from the Saudi Ministry of Health website (https://www.moh.gov.sa/en).

Data Acquisition:

Scrapy, a web scraping framework, was employed along with Beautiful Soup, a parsing library, to extract disease information from the website. The scraping process targeted three distinct layers: disease types, specific diseases within each type, and associated articles. This layered approach ensured comprehensive data capture.

Data Cleaning:

The scraped data underwent a rigorous cleaning process to prepare it for NLP tasks. This involved:

HTML Tag Removal: Eliminating extraneous HTML tags that were not relevant to the textual content.
Punctuation Removal: Removing most punctuation marks to focus on word analysis, with the exception of the shadda (تّ) which carries semantic meaning in Arabic.
Apostrophe Replacement: Replacing double quotes (") with single quotes (') to prevent accidental word merging during processing.
Whitespace Character Removal: Removing the Unicode character \u200b (zero-width space) that can introduce unwanted spaces.
Encoding Considerations:

Careful encoding practices were implemented throughout the pipeline. Data was written to JSON format using appropriate encoding to handle Arabic characters. Subsequently, the data was imported into a MongoDB NoSQL database using tools like Compass for visualization.

NLP Techniques:

This project serves as a foundation for future NLP exploration. The framework can be extended to incorporate various NLP techniques including:

Tokenization: Splitting text into individual words for analysis.
Stop Word Removal: Eliminating common words with minimal semantic value.
Stemming/Lemmatization: Reducing words to their base forms for improved analysis consistency.
Part-of-Speech (POS) Tagging: Identifying word categories (nouns, verbs, etc.) within the text.
Named Entity Recognition (NER): Recognizing and classifying named entities like disease names.
Learning Outcomes:

This project provided valuable experience in:

Web Scraping: Utilizing tools like Scrapy and Beautiful Soup for efficient data extraction.
Data Cleaning: Applying techniques to prepare textual data for NLP tasks.
NLP Concepts: Gaining exposure to fundamental NLP processes and their significance.
Encoding Practices: Understanding the importance of proper encoding for Arabic text.
Conclusion:

This project successfully established a web scraping and NLP framework for Arabic disease text data. The cleaned data and implemented functionalities provide a solid foundation for further research and the development of advanced Arabic disease classification systems.
