# Team6 RAG
2024-2 Term Project

This repository contains the final code and resources for Team 6's RAG (Retrieval-Augmented Generation) model. 

## RAG-based Solution for School Regulations and MMLU-pro

This project applies the RAG (Retrieval-Augmented Generation) technique to solve problems related to school regulations (학칙) and the MMLU-pro benchmark. The solution utilizes **Upstage's SLOAR-1-Mini-Chat** as the only model used for inference and retrieval tasks.


## Directory Structure

### `db_files/`
This folder contains the necessary database and embedding files, as well as the PDF files required to run the `Final_team6_RAG.ipynb` notebook. The files in this directory are used for data retrieval and embeddings for the RAG model.

### `db_code/`
This folder contains the Jupyter notebooks named `DB_mmlu_{}.ipynb`, where `{}` represents various domains such as law, history, business, etc. These notebooks contain the code used to generate the database and embeddings for the different domains. The notebook files process the data from the `db_files` folder to create the embeddings and database files needed for the RAG model.

### `Final_team6_RAG.ipynb`
This notebook contains the final RAG code. It integrates the database and embeddings to perform retrieval-augmented generation tasks. The code combines the outputs from the domain-specific databases with the pre-trained model to generate responses based on the input queries.


## Requirements

- A `requirements.txt` file is provided, which contains the necessary dependencies and environment settings for running the notebooks and the RAG model.
- Ensure that the environment is set up with the specified dependencies before running the notebooks.


## Installation

1. Clone this repository to your local machine:
    ```bash
    git clone https://github.com/blasiasia/ewha_nlp.git
    ```

2. Install the required dependencies:
    ```bash
    pip install -r requirements.txt
    ```

## License

This repository does not have a specified license. Please use it responsibly.
