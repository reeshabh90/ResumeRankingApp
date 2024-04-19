# Resume Ranking System

## Overview

## Part-1: sample.ipynb or directly use "get_similarity_score.py" file under scripts

## Requirements
- Python 3
- cohere
- qdrant-client
- yaml
- json
- logging

## Setup
1. Install the required packages using pip:


2. Ensure you have a valid API key for the Cohere API and Qdrant.

3. Update the configuration file `scripts/similarity/config.yaml` with your Cohere and Qdrant API keys.

## Usage
1. Provide the paths to the JSON files containing keywords extracted from resumes and job descriptions in the `READ_RESUME_FROM` and `READ_JOB_DESCRIPTION_FROM` variables, respectively.

2. Run the `app_similarity_score.py` file.

## Description
-  The Python script that calculates the similarity score between a job description and a resume using embeddings generated by the Cohere API and the Qdrant vector database.
- `config.yaml`: Configuration file containing API keys for the Cohere API and Qdrant.
- `Data/Processed/Resumes`: Directory containing JSON files with keywords extracted from resumes.
- `Data/Processed/JobDescription`: Directory containing JSON files with keywords extracted from job descriptions.
- `app_similarity_score.log`: Log file containing information about the execution of the program.


## Part-2: transformer_sample.ipynb
This project is a simple Python program that ranks resumes against a job description provided in a PDF format. It utilizes the `sentence-transformers` library for text encoding and similarity calculation, and `PyPDF2` for reading PDF documents.

## Requirements
- Python 3
- sentence-transformers
- PyPDF2

Install the required packages using pip:


## Usage
1. Place the resume PDF files in the directory specified by the `org_docs` list.
2. Provide the path to the target job description PDF file in the `target_document` variable.
3. Run the script.

## Description
-  The Python script that extracts text from PDF resumes and a job description file, encodes them into embeddings using Sentence Transformers, calculates the cosine similarity between the job description and each resume, and ranks the resumes based on their similarity scores.

## File Structure
- `Data/Resumes`: Directory containing PDF files of resumes.
- `Data/JobDescription`: Directory containing the target job description PDF file.

## License
This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.
