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
open up you local host and port
```


```bash
Author: Neeraj Manhar
IIIT Naya Raipur, Data Science and Artificial Intelligence
Email: nmanhar2002@gmail.com

```



# AWS-CICD-Deployment-with-Github-Actions

## 1. Login to AWS console.

## 2. Create IAM user for deployment

	#with specific access

	1. EC2 access : It is virtual machine

	2. ECR: Elastic Container registry to save your docker image in aws


	#Description: About the deployment

	1. Build docker image of the source code

	2. Push your docker image to ECR

	3. Launch Your EC2 

	4. Pull Your image from ECR in EC2

	5. Lauch your docker image in EC2

	#Policy:

	1. AmazonEC2ContainerRegistryFullAccess

	2. AmazonEC2FullAccess

	
## 3. Create ECR repo to store/save docker image
    - Save the URI: #####

	
## 4. Create EC2 machine (Ubuntu) 

## 5. Open EC2 and Install docker in EC2 Machine:
	
	
	#optional

	sudo apt-get update -y

	sudo apt-get upgrade
	
	#required

	curl -fsSL https://get.docker.com -o get-docker.sh

	sudo sh get-docker.sh

	sudo usermod -aG docker ubuntu

	newgrp docker
	
# 6. Configure EC2 as self-hosted runner:
    setting>actions>runner>new self hosted runner> choose os> then run command one by one


# 7. Setup github secrets:

    AWS_ACCESS_KEY_ID=

    AWS_SECRET_ACCESS_KEY=

    AWS_REGION = us-east-1

    AWS_ECR_LOGIN_URI = demo>>  723641895219.dkr.ecr.ap-south-1.amazonaws.com

    ECR_REPOSITORY_NAME = simple-app
