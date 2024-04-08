<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>Arabic Disease Text Classification Pipeline</title>
</head>
<body>

<h1>Arabic Disease Text Classification Pipeline</h1>

<p>This report details the development of a web scraping and Natural Language Processing (NLP) pipeline for Arabic disease classification, focusing on data from the Saudi Ministry of Health website (<a href="[https://www.moh.gov.sa/en](https://www.moh.gov.sa/HealthAwareness/EducationalContent/Diseases/Pages/default.aspx)">https://www.moh.gov.sa/en</a>).</p>

<h2>Data Acquisition</h2>

<p>Scrapy, a web scraping framework, was employed along with Beautiful Soup, a parsing library, to extract disease information from the website. The scraping process targeted three distinct layers:</p>

<ul>
  <li>Disease types</li>
  <li>Specific diseases within each type</li>
  <li>Associated articles</li>
</ul>

<p>This layered approach ensured comprehensive data capture.</p>

<h2>Data Cleaning</h2>

<p>The scraped data underwent a rigorous cleaning process to prepare it for NLP tasks. This involved:</p>

<ul>
  <li>HTML Tag Removal: Eliminating extraneous HTML tags.</li>
  <li>Punctuation Removal: Removing most punctuation marks, except for the shadda (تّ).</li>
  <li>Apostrophe Replacement: Replacing double quotes (") with single quotes (').</li>
  <li>Whitespace Character Removal: Removing the Unicode character \u200b.</li>
</ul>

<h2>Encoding Considerations</h2>

<p>Careful encoding practices were implemented throughout the pipeline. Data was written to JSON format using appropriate encoding to handle Arabic characters. Subsequently, the data was imported into a MongoDB NoSQL database using tools like Compass for visualization.</p>

<h2>NLP Techniques (Future Exploration)</h2>

<p>This project serves as a foundation for future NLP exploration. The framework can be extended to incorporate various NLP techniques including:</p>

<ul>
  <li>Tokenization</li>
  <li>Stop Word Removal</li>
  <li>Stemming/Lemmatization</li>
  <li>Part-of-Speech (POS) Tagging</li>
  <li>Named Entity Recognition (NER)</li>
</ul>

<h2>Learning Outcomes</h2>

<p>This project provided valuable experience in:</p>

<ul>
  <li>Web Scraping</li>
  <li>Data Cleaning</li>
  <li>NLP Concepts</li>
  <li>Encoding Practices</li>
</ul>

<h2>Conclusion</h2>

<p>This project successfully established a web scraping and NLP framework for Arabic disease text data. The cleaned data and implemented functionalities provide a solid foundation for further research and the development of advanced Arabic disease classification systems.</p>

</body>
</html>
