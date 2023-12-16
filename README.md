# NLP701-Project

## Notebooks 
**1-BigQuery-GDELT.ipynb**: This notebook is used to query the GDELT database in BigQuery in order to obtain raw event data. Approximately $1000 was spent querying the database, so this data is proprietary.

**2-scrape-GDELT.ipynb**: This notebook is used to crawl through all the links featured in the event data queried from BigQuery.

**3-format-GDELT.ipynb**: This notebook is used to reformat the columns in the event database to make it easier for manipulation and data cleaning.

**4-clean-GDELT.ipynb**: This notebook implements the data cleaning described in the Data section of the project report.

**5-linguistic-heuristic-triple-extraction.ipynb**: This notebook implements the triple extraction algorithms described in the Methods section of the project report.

**6-train-triple-extraction-transformer.ipynb**: This notebook trains the triple extraction model with token classification as described in the project report.

**7-train-Goldstein_regression_model.ipynb**: This notebook trains the transformer-based regression model as described in the project report.

**8-NER-extraction.ipynb**: This notebook extracts NERs from the subjects and objects in triples.

**9-test-trained-models.ipynb**: Use this notebook to freely test the trained models

**Exxon.html** - A sample network of RDF triples extracted using the triple parsing model

**Royce.html** - A sample network of RDF triples extracted using the triple parsing model

## Datasets and Models
The datasets used to train the token classification models, as well as the trained models are all contained in the following Google Drive Repository: https://drive.google.com/drive/folders/1YUGJwoRSQg0ukqSyafNzl_4CuVtwm_el?usp=drive_link

The files included are: 

**tokenizer2** - tokenizer for the Goldstein regression model

**model2** - the Goldstein regression model

**model-best** - the triple extraction model

**base_config.cfg** - the base configuration for the Spacy token classification framework used to train the triple extraction model

**train.spacy** - the dataset used to train the token classification model

**scraped_goldstein_filtered.fthr** - the dataset used to train the goldstein regression model

## Dependencies

! pip install -U torch
! pip install -U transformers
! pip install -U datasets
! pip install sentencepiece
! pip install transformers[torch]
! pip install numba
! pip install spacy
! pip install spacy-transformers
