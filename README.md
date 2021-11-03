# cutie-for-invoices
Deep neural network to extract intelligent information from invoice documents using PyTorch.

In this project we implement the CUTIE Model for invoices. https://arxiv.org/abs/1903.12363

====================================
In order to detect and extract total amount TTC information on receipt document, we will train a deep learning model with a labeled database containing the receipts and their corresponding labels (which are in our case mask*). In the following section, some tasks are enumerated.

Annotate the receipts in order to build the masks (Labels), for this task we will use LabelImg (https://github.com/tzutalin/labelImg).
As the textual information is nedded, we will process OCR to extract the text from the images. We will use Pytesseract.(https://pypi.org/project/pytesseract/)
Doing some feature engineering on the text (Cleaning, tokenization ...), Nltk and gensim ar used.
Pytorch transformation, PIL and CV2 are used to process the images (receipts and grids)
Pytorch is used to train the deep learning model.
mask*: image with 1 for the position of 'total' in the receipt, and 0 elsewhere.


Key words: Deep Learning, PyTorch, NLP, NLTK, Text processing, OCR, Pytesseract, Image, Information Retreival
