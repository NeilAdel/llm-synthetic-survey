**Using Large Language Models to Simulate Consumer Expectations**

## Overview

This repository contains code and ongoing research materials for a project investigating whether Large Language Models (LLMs) can reproduce patterns observed in real-world consumer expectation surveys.

The project builds on the methodological framework proposed by **Wu, Xi and Xie (2025)** and adapts it to the University of Michigan Survey of Consumers, focusing initially on consumer expectations about gasoline prices.

The broader objective is to investigate how LLM-generated synthetic respondents can reproduce human survey responses, and to understand the limitations and potential of LLMs as tools for survey-based research.

## Research Objectives

The project focuses on:

- Replicating and adapting an existing LLM-based survey methodology.
- Constructing synthetic respondents using survey and demographic information.
- Controlling the information available to synthetic respondents to reduce potential knowledge contamination.
- Comparing LLM-generated responses with actual responses from human survey participants.
- Evaluating response patterns and differences across questions and survey periods.

## Empirical Application: University of Michigan Survey of Consumers

The initial empirical application uses four gasoline price expectation questions from the University of Michigan Survey of Consumers.

| Variable | Description |
|---|---|
| GASPX1 | Expected direction of gasoline prices over five years |
| GASPX2 | Expected magnitude of five-year price change |
| GAS1PX1 | Expected direction of gasoline prices over twelve months |
| GAS1PX2 | Expected magnitude of twelve-month price change |

The historical survey data cover multiple decades, although the availability of these questions varies across survey periods. Identifying comparable waves and understanding the structure of the original questionnaire are therefore important parts of the research.

**Exploratory Data Analysis:** [Michigan Survey EDA Dashboard](https://neiladel.github.io/EDA-UMICH/)

## Repository Structure

The repository is organised around the main stages of the research:

```text
llm-synthetic-survey-research/
│
├── README.md
│
├── 01_michigan_survey_eda/
│   └── exploratory_analysis.ipynb
│
├── 02_persona_extraction/
│   └── persona_extraction.py
│
├── 03_knowledge_restriction/
│   └── knowledge_restriction.py
│
├── 04_survey_pilot/
│   └── pilot_experiment.py
│
└── requirements.txt
```

*The structure will evolve as the research progresses.*

## Current Implementation

The repository currently contains work on the following components:

**1. Exploratory Data Analysis**

Exploration of the Michigan Survey of Consumers, including variable identification, question availability, response distributions and temporal patterns.

**2. Synthetic Persona Extraction**

Python code for extracting and constructing synthetic respondent personas using available respondent characteristics and survey information.

**3. Knowledge Restriction**

An approach to restricting the information available to LLM-generated respondents, with the aim of reducing reliance on knowledge beyond the information intended to be available to them.

**4. Pilot Survey Implementation**

Initial experiments testing the implementation of the gasoline price expectation questions with LLM-generated respondents.

These components represent ongoing research and preliminary implementation rather than a completed or fully validated survey simulation framework.

## Methodological Direction

The project follows the LLM survey framework proposed by Wu, Xi and Xie (2025), with an initial focus on adapting its methodology to an established consumer expectations survey.

The validation strategy aims to compare synthetic responses with real human survey evidence, examining response distributions, aggregate patterns and differences across survey questions and periods.

## Future Development: Agentic Research Workflow

An important direction for future development is introducing an agentic layer to support and automate different stages of the research pipeline.

Potential applications include:

- Automated literature extraction and evidence verification.
- Survey data auditing and quality assurance.
- Automated execution and validation of analytical workflows.
- Monitoring response patterns and inconsistencies across survey waves.
- Reproducible documentation of experiments, model configurations and results.

The longer-term ambition is to develop a framework capable of running synthetic surveys periodically and systematically evaluating their outputs against real-world survey benchmarks.

This agentic extension is an ongoing development direction and is not yet implemented.

## Technologies

- Python
- Pandas and NumPy
- Statistical and exploratory data analysis
- Large Language Models and API-based inference
- Jupyter Notebooks

## Research Status

**Work in progress.**

The current focus is on methodological replication, survey data exploration and pilot implementation. Further development will address systematic validation against human survey responses and the integration of agentic workflows.

## Research Motivation

This project aims to contribute to the emerging field of LLM-based survey research by examining whether synthetic respondents can reproduce meaningful patterns in real human survey data.

Rather than treating LLM-generated responses as substitutes for human participants, the research investigates their capabilities, limitations and potential applications as tools for computational social science.

## Author

**Niloofar Adel**

Junior Researcher & Data Scientist  
Fondazione Eni Enrico Mattei (FEEM)

[GitHub](https://github.com/neiladel)

---

*This repository is part of an ongoing research project. Methodologies, code and results are subject to further development.*
