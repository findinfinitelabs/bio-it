# FindInfinite Labs Presents at Bio-IT World Congress 2025
Accelerating Drug Discovery and Biomarker Mapping through the Convergence of Quantum Computing and AI for the 2025 Bio-IT World Congress in Boston, MA. 

## Requirements

To run the code in this project, you need to have the following libraries installed:

- `torch`
- `transformers`
- `huggingface_hub`
- `requests`
- `beautifulsoup4`
- `lxml`
- `pandas`

You can install these libraries using pip:

```sh
pip install torch transformers huggingface_hub requests beautifulsoup4 lxml pandas
```

## Python Environment

This project is developed using Python 3.9.6. Ensure you have this version or a compatible version of Python installed.

### Code Setup

The main code is located in the gene-expression.ipynb file. This Jupyter notebook performs the following tasks:

- Load BioBERT: Load the BioBERT model pre-trained for biomedical Named Entity Recognition (NER).
- Fetch PubMed Abstracts: Fetch sample PubMed abstracts related to breast cancer biomarkers.
- Extract Entities: Process the text with BioBERT to extract entities such as genes or proteins.
- Load GEO/TCGA Data: Load sample GEO/TCGA data (mocked for demo purposes).
- Main Discovery Logic: Identify potential biomarkers by matching extracted entities with GEO/TCGA data.
- Rank by Expression Difference: Rank the potential biomarkers by their expression difference.

### Datasets

The notebook uses the following datasets:

PubMed Abstracts: Fetched dynamically using the NCBI E-utilities API.
GEO/TCGA Data: Mocked data for demonstration purposes. Replace with real data as needed.

### Running the Notebook

To run the notebook, follow these steps:

1. Install the required libraries using the pip command provided above.
2. Open the gene-expression.ipynb file in Jupyter Notebook or JupyterLab.
3. Execute the cells in the notebook sequentially to perform the analysis.

### Example Output

The notebook will output a list of potential biomarkers for breast cancer along with their expression differences. Here is an example of the output:

### Example Output

```python
Potential Biomarkers for Breast Cancer:
Empty DataFrame
Columns: [Gene, Expression_Diff]
Index: []
```

> Note: The output is based on the mocked data provided in the notebook. Replace the mocked data with real GEO/TCGA data for meaningful results.