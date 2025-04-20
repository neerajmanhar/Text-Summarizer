# End to end Text-Summarizer-Project

## Overview
This project is a **text summarization tool** leveraging Google's **PEGASUS model** to generate high-quality **abstractive summaries**. The model is integrated with a **Flask API**, and the application is deployed on **AWS** using **CI/CD** pipelines.

## Features
- **Abstractive Summarization**: Generates human-like summaries rather than just extracting key sentences.
- **Flask API**: Provides an easy-to-use RESTful interface.
- **AWS Deployment**: Hosted using **CI/CD pipelines** for automated updates.
- **Dockerized**: Packaged with **Docker** for easy containerized deployment.
- **User-Friendly**: Simple input-output mechanism via API calls.

## Tech Stack
- **Model**: Google's [PEGASUS](https://arxiv.org/abs/1912.08777) for text summarization
- **Backend**: Flask (Python)
- **Deployment**: AWS (Elastic Beanstalk, CI/CD)
- **Containerization**: Docker
- **Version Control**: GitHub


## Workflows

1. Update config.yaml
2. Update params.yaml
3. Update entity
4. Update the configuration manager in src config
5. update the conponents
6. update the pipeline
7. update the main.py
8. update the app.py


# How to run?
### STEPS:

Clone the repository

```bash
https://github.com/neerajmanhar/Text-Summarizer
```
### STEP 01- Create a conda environment after opening the repository

```bash
conda create -n summary python=3.8 -y
```

```bash
conda activate summary
```


### STEP 02- install the requirements
```bash
pip install -r requirements.txt
```


```bash
# Finally run the following command
python app.py
```

Now,
```bash
open up your local host and port
```


```bash
Author: Neeraj Manhar
IIIT Naya Raipur, Data Science and Artificial Intelligence
Email: nmanhar2002@gmail.com

