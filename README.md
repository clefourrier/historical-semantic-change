# Repository for the 2022 L'Change paper "Caveats of Measuring Semantic Change of Cognates and Borrowings using Multilingual Word Embeddings"
Clémentine Fourrier and Syrielle Montariol.

## Organisation
This repository contains two main folders:
- **cognates_and_borrowings**, which contains 
	- **WiktionaryParser.ipynb**, a jupyter notebook with the cognate and borrowings extraction scripts
	- **cognates_large_uniq_cog/bor_manual.csv**, manually cleaned cognates/borrowings datasets after extraction
- **embeddings**, which contains 
	- **historical_datasets**, the cleaned datasets we used to build the embedding spaces for the historical languages, in old Spanish (osp) and medieval French (frm)
	- **extracted_embeddings**, the extracted embeddings we generated, for fasttext and bert, with a notebook to display similarity scores, called **EmbeddingsAnalysis.ipynb**

## Using the scripts
### Wiktionary extractor
To use the WiktionaryParser script, you need to have Python3 and Jupyter installed. It uses unidecode and unicodedata Python libs. 
Then, you need to download the current version of the Wiktionary article pages data dump, which should be named "enwiktionary-latest-pages-articles.xml", and save it in the script folder. Extraction will take some time to run.

### Embeddings Analysis 
To use the WiktionaryParser script, you need to have Python3 and Jupyter installed. It uses pickle, scipy, pandas and numpy Python libs. 


## Licence
This repo and its code is CC BY-NC-SA.

The datasets in embeddings/historical_datasets/frm are CC BY or CC BY-NC-SA by the original authors of LEM17, MCVF 1.0 and 2.0, PPCHF 1.0, OpenMedFr and BFM2019. All attribution is made in the original paper available along the code.