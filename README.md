# Team6 RAG
2024-2 Term Project
This repository contains the final code and resources for Team 6's RAG (Retrieval-Augmented Generation) model.

## Directory Structure

### `db_files/`
This folder contains the necessary database and embedding files, as well as the PDF files required to run the `Final_team6_RAG.ipynb` notebook. The files in this directory are used for data retrieval and embeddings for the RAG model.

### `db_code/`
This folder contains the Jupyter notebooks named `DB_mmlu_{}.ipynb`, where `{}` represents various domains such as law, history, business, etc. These notebooks contain the code used to generate the database and embeddings for the different domains. The notebook files process the data from the `db_files` folder to create the embeddings and database files needed for the RAG model.

### `Final_team6_RAG.ipynb`
This notebook contains the final RAG code for Team 6. It integrates the database and embeddings to perform retrieval-augmented generation tasks. The code combines the outputs from the domain-specific databases with the pre-trained model to generate responses based on the input queries.

## Requirements

- A `requirements.txt` file is provided, which contains the necessary dependencies and environment settings for running the notebooks and the RAG model.
- Ensure that the environment is set up with the specified dependencies before running the notebooks.

## How to Run

1. Clone this repository to your local machine:
    ```bash
    git clone <repository_url>
    ```

2. Install the required dependencies:
    ```bash
    pip install -r requirements.txt
    ```

3. To generate the embeddings and database, run the domain-specific notebooks from the `db_code/` folder:
    ```bash
    jupyter notebook db_code/DB_mmlu_law.ipynb
    jupyter notebook db_code/DB_mmlu_history.ipynb
    jupyter notebook db_code/DB_mmlu_business.ipynb
    ```

4. Once the databases and embeddings are ready, you can run the final RAG model:
    ```bash
    jupyter notebook Final_team6_RAG.ipynb
    ```

## License

This repository is licensed under the MIT License. See the LICENSE file for more details.
