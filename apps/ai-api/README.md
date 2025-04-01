# ai-api (FastAPI)

This directory contains the FastAPI app for AI or ML endpoints.

## Virtual Environment Activation

To activate the virtual environment, run:

```bash
source /Users/trongphan/Desktop/LinkediNTU/apps/ai-api/venv/bin/activate
```
Installation
We are using Poetry as the package manager for this project. To install the dependencies, run:

```bash
poetry install
```

Then, activate the virtual environment with:

```bash
poetry shell
```

## Running the App
>> Note: This part is still under development and may not be fully functional yet.

To run the app, use the following command:

```bash
uvicorn app.main:app --reload
```

## Project Structure
The project structure is as follows:

```bash
ai-api/
├── app                # Contains the FastAPI application (and UI)
├── training
│   ├── augmentor      # Data augmentation scripts
│   └── finetuning     # Fine-tuning scripts for models
├── utils
│   ├── analyser
│   │   ├── prompts.txt
│   │   └── resume_analyser.py  # Analyze resumes using LLMs
│   ├── data
│   │   ├── feedback          # Stores feedback in JSON format
│   │   ├── processed_resume  # Stores parsed resumes in JSON format
│   │   └── resume_pdf
│   ├── parser
│   │   └── ResumeParser.py   # Resume Parser class
│   └── section_classifier
│       └── (description pending)
└── venv               # Virtual environment directory
```
