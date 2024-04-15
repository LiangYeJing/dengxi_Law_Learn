# Central South Railway Guerrillas

## ChatLaw3 and privateGPT Deployment Guide

This guide provides detailed instructions for deploying and using the ChatLaw3 and privateGPT large models on Alibaba Cloud ECS servers and PAI DSW, tailored for enhancing security and functionality in intelligent home systems, particularly for single young female users.

### Table of Contents

- [ChatLaw3 Deployment](#chatlaw3-deployment)
  - [System Requirements](#system-requirements)
  - [Configuration Requirements](#configuration-requirements)
  - [API Execution](#api-execution)
- [privateGPT Deployment](#privategpt-deployment)
  - [System Requirements](#system-requirements-1)
  - [Configuration Requirements](#configuration-requirements-1)
  - [Execution](#execution)
- [Important Notes](#important-notes)

## ChatLaw3 Deployment

### System Requirements

- **Operating System:** Linux
- **Python Version:** 3.7 or higher

### Configuration Requirements

Ensure the following Python packages are installed:

- protobuf>=4.25.3
- transformers>=4.38.1
- tokenizers>=0.15.0
- cpm_kernels>=1.0.11
- torch>=2.1.0
- gradio>=4.19.2
- sentencepiece>=0.2.0
- sentence_transformers>=2.4.0
- accelerate>=0.27.2
- streamlit>=1.31.0
- fastapi>=0.109.0
- loguru~=0.7.2
- mdtex2html>=1.3.0
- latex2mathml>=3.77.0
- jupyter_client>=8.6.0
- openai>=1.12.0
- zhipuai>=2.0.1
- pydantic>=2.6.2
- sse-starlette>=2.0.0
- uvicorn>=0.27.1
- timm>=0.9.12
- tiktoken>=0.6.0
- langchain>=0.1.9
- langchainhub>=0.1.14
- arxiv>=2.1.0

### API Execution

Execute the following command on your Alibaba Cloud ECS server to start the API server for ChatLaw3:

```bash
$ python ChatLaw3/openai_api_demo/api_server.py

### privateGPT Deployment

System Requirements
Operating System: Linux
Python Version: 3.6 or higher
Configuration Requirements
Install the following packages:

- langchain==0.0.274
- gpt4all==1.0.8
- chromadb==0.4.7
- llama-cpp-python==0.1.81
- urllib3==2.0.4
- PyMuPDF==1.23.1
- python-dotenv==1.0.0
- unstructured==0.10.8
- extract-msg==0.45.0
- tabulate==0.9.0
- pandoc==2.3
- pypandoc==1.11
- tqdm==4.66.1
- sentence_transformers==2.2.2

Execution
Run privateGPT on your system by executing:
$ python privateGPT/privateGPT.py

Important Notes
Ensure all necessary packages are installed in your Python environment before running the models.
Proper permissions and configurations must be set up on your Alibaba Cloud ECS server and PAI DSW for smooth execution.
ChatGLM3-6B model files can be downloaded from the ChatGLM3 GitHub repository, and the tuned large language legal model files are located in the chatglm3-6b directory.
privateGPT model files are available in the private-gpt GitHub repository.
Refer to other materials\2403031-Central South Railway Guerrillas-[A29] AI Makes Life Easier-Data Sets\Private Knowledge Database for private database details. """
Saving the content to a Markdown (.md) file
file_path = "/mnt/data/README.md" with open(file_path, "w") as file: file.write(readme_content)

file_path
