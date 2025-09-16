# Evaluation of a Small Language Model on Persian BoolQA Using lm-eval-harness

## Project Overview

This project focuses on evaluating a small language model on the **BoolQA (Persian)** dataset using [lm-eval-harness](https://github.com/EleutherAI/lm-eval-harness). The goal is to establish a reproducible and extensible evaluation pipeline that extracts standard performance metrics such as **Accuracy**, **F1 Score**, and **Mean Score**, and assesses the model’s ability to perform semantic understanding and logical inference in Persian.

The workflow includes setup, execution, result collection, reporting, and Git integration with clear structure and automation support.

## Dataset: BoolQA (Persian)

**BoolQA** is a yes/no question-answering dataset in Persian, designed to test the logical and semantic reasoning capabilities of language models.
Each example includes:

* A short context (sentence or paragraph)
* A question
* A binary answer: “Yes” or “No” (in Persian: “بله” or “خیر”)

Although seemingly simple, the dataset challenges models to avoid superficial inference and instead demonstrate true understanding and attention to detail.

**Note**: A sample dataset is included.
For access to the full dataset, please contact via email (ailabs@itrc.ac.ir)

## Setup Instructions

### Requirements

* Python >= 3.8
* pip >= 20
* Virtual environment (recommended)

### Installation

```bash
git clone https://github.com/ItrcAiLabs/Evaluating-the-LLM-Internship-Task-
cd Evaluating-the-LLM-Internship-Task-

# Create and activate virtual environment
python -m venv .venv
source .venv/bin/activate  # On Windows: .venv\Scripts\activate

# Install dependenciesif you have create requirements.txt
pip install -r requirements.txt
```

## Code Structure

The project is implemented with a **modular and extensible structure**, supporting clean separation of concerns across:

* Data preparation
* Model evaluation
* Metrics logging
* Testing
* CI/CD integration


## Metrics Computed:

   * Accuracy
   * F1 Score
   * Mean Score
   * (Optional) Sample-wise outputs

## CI/CD and Automation

This project integrates **GitHub Actions** to enforce code quality and reproducibility. The CI pipeline includes:

* Linting and code style checks
* Unit tests
* Secure file handling validation

## Testing

Unit tests are implemented using `pytest`. To run tests:

```bash
pytest tests/
```

## Security Guidelines

* Sensitive information (e.g., API keys, server credentials) must be stored in secure files (e.g., `.env`) and excluded from version control.
* `.gitignore` is configured accordingly to prevent accidental exposure of secrets.

## Reporting and Deliverables

At the conclusion of evaluation, a report will be generated including:

* Summary of evaluation metrics
* Observed challenges or issues during the process
* Suggestions for improving evaluation quality or model performance
* (If applicable) comparisons across models

## Deliverables

* Evaluation scripts and configuration
* Preprocessing tools (if required)
* Evaluation results in structured format (e.g., JSON)
* Unit tests and validation
* README and documentation
* CI/CD pipeline via GitHub Actions
* A complete pull request (PR) with a clear description and instructions for review and reproducibility

