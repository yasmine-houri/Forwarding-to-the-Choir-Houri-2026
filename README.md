# Replication Materials

Replication materials for:

**Houri, Y. (2026).** Forwarding to the choir: topic assortativity in far-right Telegram networks. *Applied Network Science*.

This repository contains the Python notebooks and derived analytical materials accompanying the paper. It documents the use of large language models (LLMs) for topic annotation, the validation of LLM-generated annotations against human annotations, the computational analyses combining natural language processing (NLP) and social network analysis (SNA), and the statistical validations of these analyses.

## Repository Structure

```text
.
├── data/
│   ├── graph.gexf
│   └── topic_prevalence.csv
│
├── code/
│   ├── mistral_annotation.ipynb
│   ├── replication_notebook.ipynb
│   └── statistical_validations.ipynb
│
├── README.md
├── requirements.txt
```

### Data

The `data/` directory contains derived analytical materials used in the paper:

- **`graph.gexf`**: Network of forwarded Telegram messages used in the social network analysis.
- **`topic_prevalence.csv`**: Topic prevalence vectors derived from the LLM-based annotation and subsequent data-processing procedures.

The original Telegram message-level dataset is sampled from the [Pushshift Telegram dataset][https://zenodo.org/records/3607497]. It is not included in this repository. Consequently, reproducing the complete analytical pipeline from the original messages requires access to the underlying data.

Further information about the available data files is provided in `data/README.md`.

### Code

The `code/` directory contains three Jupyter notebooks documenting the computational workflow:

- **`mistral_annotation.ipynb`**: Documents and implements the LLM-based topic annotation procedure using the Mistral API, including the annotation prompts and relevant model configuration.
- **`statistical_validations.ipynb`**: Reproduces the two statistical tests used to assess the validity of LLM-generated topic annotations against human annotations.
- **`replication_notebook.ipynb`**: Reproduces the main analyses reported in the paper, combining NLP and SNA.

## Reproducibility

The repository provides the analytical code and derived materials used in the study to facilitate methodological transparency and independent inspection of the research workflow.

The main analytical and statistical validation procedures can be inspected through the corresponding notebooks. However, reproducing the complete pipeline from the original Telegram messages requires access to the underlying message-level dataset, which is not redistributed here.

Re-executing the LLM annotation procedure requires a Mistral API key and may incur API usage costs. The original annotations used in the study were generated through the Mistral API. As the procedure relies on an externally hosted proprietary model, exact reproduction of the original outputs is not guaranteed.

## Requirements

The notebooks are written in Python and use the libraries specified in `requirements.txt`.

To install the dependencies:

```bash
pip install -r requirements.txt
```

To execute the Mistral annotation notebook, a valid Mistral API key must also be configured as an environment variable. No API credentials are included in this repository.

## Citation

If you use this repository or build upon its materials, please cite the associated publication:

Houri, Y. (2026). Forwarding to the choir: topic assortativity in far-right Telegram networks. *Applied Network Science*.

## Contact

For questions concerning the replication materials or methodological procedures, please contact the author.
