# 中南铁道游击队
## ChatLaw3 和 privateGPT 部署指南

本 README 提供了在阿里巴巴云 ECS 服务器和 PAI DSW 上部署和使用两个大型模型 ChatLaw3 和 privateGPT 的说明。

### 目录

- [ChatLaw3 部署](#chatlaw3-部署)
  - [系统要求](#系统要求)
  - [配置要求](#配置要求)
  - [API 执行](#api-执行)
- [privateGPT 部署](#privategpt-部署)
  - [系统要求](#系统要求-1)
  - [配置要求](#配置要求-1)
  - [执行](#执行)
- [重要注意事项](#重要注意事项)

### ChatLaw3 部署

#### 系统要求

- 操作系统：Linux
- Python 版本：3.7 或更高

#### 配置要求

需要以下 Python 包：

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
- **ChatGLM3-6B**: 模型权重可以从 [这里](https://github.com/THUDM/ChatGLM3) 下载。请确保在这个 [网站](chatglm3-6b) 上对大型语言法律模型文件权重进行微调。

#### API 执行

要在 ECS 服务器上运行 ChatLaw3 的 API 服务器，请在终端中执行以下命令：

```shell
$ python ChatLaw3/openai_api_demo/api_server.py


