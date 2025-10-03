# CanRace RAG Business Rules Pipeline

This repository implements a Retrieval-Augmented Generation (RAG) pipeline to validate racing eligibility logic for CanRace entities such as horses, jockeys, trainers, and owners.

##  Purpose

The goal is to ensure that prompts related to racing eligibility correctly retrieve rule-based chunks using semantic search and ontology tagging.

##  Folder Structure

canrace-rag-business-logic/ ├── README.md ├── rule_chunks.yaml ├── ontology_schema.yaml ├── test_prompts.yaml ├── expected_chunks.yaml ├── qa_runner.py ├── test_log.csv └── prompt_templates.yaml



##  File Descriptions

- `rule_chunks.yaml`: Contains rule logic chunks with metadata
- `ontology_schema.yaml`: Defines the schema for tagging entities and flags
- `test_prompts.yaml`: Negative test prompts to challenge the RAG system
- `expected_chunks.yaml`: Expected rule chunks for each test prompt
- `qa_runner.py`: Python script to run QA tests and log results
- `test_log.csv`: Output log of test results
- `prompt_templates.yaml`: Generalized prompt templates for rule validation

##  How to Use

1. Clone the repo
2. Run `qa_runner.py` to validate prompt-to-chunk retrieval
3. Review `test_log.csv` for pass/fail results

##  QA Focus

- Entity-specific rule enforcement
- Ontology-based chunk retrieval
- Prompt accuracy and coverage

##  Entities Covered

- Horse
- Jockey
- Trainer
- Owner
