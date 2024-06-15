# Generative-AI-with-AWS

# Meta Llama 2 7B Model Fine-Tuning Project

This repository contains the code and documentation for fine-tuning the Meta Llama 2 7B model on a medical domain dataset using Amazon SageMaker. The project involves setting up the model, evaluating its initial performance, fine-tuning it with domain-specific data, and comparing the results.

## Concepts

### 1. Fine-Tuning
Fine-tuning is the process of taking a pre-trained language model and retraining it on a specific dataset related to a particular task or domain. This allows the model to leverage its existing knowledge while adapting to new, domain-specific information.

### 2. Large Language Models (LLMs)
Large Language Models, such as Meta Llama 2 7B, are neural networks trained on vast amounts of text data. These models can generate coherent and contextually relevant text by predicting the next word in a sequence based on the input provided.

### 3. Amazon SageMaker
Amazon SageMaker is a fully managed service that provides every developer and data scientist with the ability to build, train, and deploy machine learning models quickly. It allows for easy integration and deployment of machine learning models at scale.

## Project Overview

### Step 1: Domain Choice
For this project, we chose the **medical** domain for fine-tuning the Meta Llama 2 7B model.

### Step 2: Model Evaluation
We first deployed the pre-trained Meta Llama 2 7B model using Amazon SageMaker and evaluated its initial performance on domain-specific inputs.

**Example Input and Pre-trained Model Response:**
- **Input:** "Genomic characterization is essential for"
- **Response:** "the development of a successful vaccine and treatment strategy. Early identification of the pathogen and its antigenic profile is important for the development of an effective vaccine and treatment. The emergence of the new coronavirus has led to a pandemic of unprecedented magnitude."

### Step 3: Fine-Tuning
We fine-tuned the model using a medical domain dataset stored in an S3 bucket. The fine-tuning process was executed using Amazon SageMaker's JumpStart Estimator.


### Step 4: Fine-Tuned Model Evaluation
After fine-tuning, we deployed the updated model and evaluated its performance using the same domain-specific inputs.

**Example Input and Fine-Tuned Model Response:**
- **Input:** "Genomic characterization is essential for"
- **Response:** "[{'generated_text': ' the identification of the pathogenic genes in the etiology of genetic disorders. Genome-wide association studies (GWAS) are a powerful tool for the identification of the genetic variants associated with the development of diseases. In this study, we have used GWAS to identify the'}]"

### Conclusion
The fine-tuned model showed improved domain-specific knowledge and provided more relevant and detailed responses to medical domain prompts compared to the pre-trained model. This demonstrates the effectiveness of fine-tuning large language models on specific datasets to enhance their performance in targeted areas.
