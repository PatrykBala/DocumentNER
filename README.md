# Document NER
Master's thesis defense project.
## General info
The classic method of processing and extracting text from an image (OCR) in cooperation with the *Entity Recognition* (NER) technology in a trained algorithm based on a set of business cards.

<sub> PL: Klasyczna metoda przetwarzania oraz wyodrębniania tekstu z obrazu (OCR) we współpracy z technologią rozpoznawania jednostek (NER) w przeszkolonym algorytmie na podstawie zbioru wizytówek. </sub>

## Technologies
&emsp;Python<br> 
&emsp;Jupyter Notebook<br> 
&emsp;OCR<br>
&emsp;&emsp;OpenCV<br>
&emsp;&emsp;Tesseract OCR<br>
&emsp;NER<br>
&emsp;&emsp;Pandas<br>
&emsp;&emsp;SpaCy<br>
&emsp;&emsp;RegEx<br>

## Solution architecture
Computer vision scans the document, identifies the position of the text and eventually extracts the text from the image. Natural language processing extracts units from text. The document in image form is read using OCR technology to extract text in editable form. The extracted text is cleaned and passed to a learning model that is trained to recognize names. Finally, the named units from this model will be generated.
![image](https://github.com/PatrykBala/DocumentNER/assets/73967948/a12a8f79-86b8-4f90-8048-f5f98fef9e0b)

## Scheme of the process
The scheme of the process and the operation of the application can be described in ten steps:
1. The process of sending documents via desktop or mobile devices.
2. Paper documents, submissions and emails containing scans or photos documents.
3. A collection of a certain number of files containing documents as a base.
4. The process of analyzing photos and scans of documents by OCR technology.
5. Extraction of text from the document base.
6. Generation of text data and preprocessing and data cleaning.
7. Labeling test data with the BIO system for training the NER model.
8. NER model training process.
9. Extracting text data with named units from documents.

## Setup
**Use** a single pipeline code file named *predictions.py*, with all the necessary functions. Comments are included in the code.
![image](https://github.com/PatrykBala/DocumentNER/assets/73967948/68251d11-46e9-46fc-9a06-4e5e5c1c66bb)
