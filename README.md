# NLP701-Project

1-BigQuery-GDELT.ipynb: This notebook is used to query the GDELT database in BigQuery in order to obtain raw event data. Approximately $1000 was spent querying the database, so this data is proprietary.

2-scrape-GDELT.ipynb: This notebook is used to crawl through all the links featured in the event data queried from BigQuery.

3-format-GDELT.ipynb: This notebook is used to reformat the columns in the event database to make it easier for manipulation and data cleaning.

4-clean-GDELT.ipynb: This notebook implements the data cleaning described in the Data section of the project report.

5-linguistic-heuristic-triple-extraction.ipynb: This notebook implements the triple extraction algorithms described in the Methods section of the project report.

6-train-triple-extraction-transformer.ipynb: This notebook trains the triple extraction model with token classification as described in the project report.

7-train-Goldstein_regression_model.ipynb: This notebook trains the transformer-based regression model as described in the project report.

8-NER-extraction.ipynb: This notebook extracts NERs from the subjects and objects in triples.
