# 邓析法学大模型服务端README

此README提供了在阿里巴巴云ECS服务器和PAI DSW上部署和使用两个大型模型，ChatLaw3和privateGPT的指南。

## 目录

- [ChatLaw3 部署](#chatlaw3-部署)
  - [系统要求](#系统要求)
  - [配置要求](#配置要求)
  - [API 执行](#api-执行)
- [privateGPT 部署](#privategpt-部署)
  - [系统要求](#系统要求-1)
  - [配置要求](#配置要求-1)
  - [执行](#执行)
- [重要提示](#重要提示)

## ChatLaw3 部署
  
  模型代码请见：https://github.com/THUDM/ChatGLM3
  
  本模型文件即chatglm3-6b
  
### 系统要求

- 操作系统：Linux
- Python版本：3.7或更高

### 配置要求

需要以下Python包：

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

### API 执行

在您的ECS服务器上执行以下命令以运行ChatLaw3的API服务器：

```bash
$ python ChatLaw3/openai_api_demo/api_server.py
```

## privateGPT 部署
  模型代码请见：https://github.com/zylon-ai/private-gpt
  本模型文件请见：https://modelscope.cn/models/Fengshenbang/Ziya-LLaMA-13B-v1/summary
### 系统要求

- 操作系统：Linux
- Python版本：3.6或更高

### 配置要求

需要以下Python包：

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

### 执行

在您的系统上执行以下命令以运行privateGPT：

```bash
$ python privateGPT/privateGPT.py
```

## 重要提示

- 在运行模型前，请确保已在您的Python环境中安装了必要的包。
- 确保在阿里巴巴云ECS服务器和PAI DSW上已设置好适当的权限和配置，以确保模型的顺利执行。

