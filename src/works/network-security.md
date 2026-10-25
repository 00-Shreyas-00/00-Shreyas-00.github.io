---
title: Network Security MLOps
order: 5
featured: true
year: 2024
category: MLOps
stack: Python, scikit-learn, MLflow, FastAPI, Docker, AWS
thumbLabel: MLflow · FastAPI · AWS
summary: An end-to-end MLOps project on phishing data, with a modular training pipeline, MLflow experiment tracking, a FastAPI service and a CI/CD workflow that pushes a Docker image to AWS ECR.
repo: https://github.com/00-Shreyas-00/Network-Secutity
---

## Pipeline

### From ingestion to a trained model

Data is ingested from MongoDB, validated against a schema with a data-drift report, transformed and used to train a scikit-learn model. Experiments are tracked with MLflow on DagsHub, and pipeline artifacts can be synced to Amazon S3.

## Serving and delivery

### FastAPI, Docker and GitHub Actions

A FastAPI application triggers training and serves predictions from the saved model. A GitHub Actions workflow lints and tests the code, then builds the Docker image and pushes it to Amazon ECR.
