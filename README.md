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

**Exploratory Data Analysis:** [Michigan Survey EDA Dashboard]([https://neiladel.github.io/EDA-UMICH/](https://neiladel.github.io/llm-synthetic-survey/01_michigan_survey_eda/))

## Repository Structure

The repository is organised around the main stages of the research:

```text
llm-synthetic-survey-research/
│
├── README.md
│
├── 01_michigan_survey_eda/
│  ├── data.json
│  ├── index.html
│
└── 02_pilot_experiment/
    ├── README.md
    ├── persona_extraction.ipynb
    ├── knowledge_restriction.ipynb
    └── survey.ipynb

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

**4. Pilot Survey Implementation (in progress)**

Initial experiments testing the implementation of the gasoline price expectation questions with LLM-generated respondents.

These components represent ongoing research and preliminary implementation rather than a completed or fully validated survey simulation framework.

## Methodological Direction

The project follows the LLM survey framework proposed by Wu, Xi and Xie (2025), with an initial focus on adapting its methodology to an established consumer expectations survey.

The validation strategy aims to compare synthetic responses with real human survey evidence, examining response distributions, aggregate patterns and differences across survey questions and periods.

## Research Status

**Work in progress.**

The current focus is on methodological replication, survey data exploration and pilot implementation. Further development will address systematic validation against human survey responses and the integration of agentic workflows.

## Research Motivation

This project aims to contribute to the emerging field of LLM-based survey research by examining whether synthetic respondents can reproduce meaningful patterns in real human survey data.

Rather than treating LLM-generated responses as substitutes for human participants, the research investigates their capabilities, limitations and potential applications as tools for computational social science.

## Author

**Niloofar Adel**

Junior Data Scientist & Researcher
Fondazione Eni Enrico Mattei (FEEM)

[GitHub](https://github.com/neiladel)

---

*This repository is part of an ongoing research project. Methodologies, code and results are subject to further development.*
