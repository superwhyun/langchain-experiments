# LangChain Experiments
이 리포지토리는 대규모 언어 모델(LLM)로 강력한 애플리케이션을 구축하기 위한 LangChain 라이브러리 실험에 중점을 두고 있습니다. 이 프로젝트는 OpenAI의 GPT-3.5 Turbo(및 곧 출시될 GPT-4)와 같은 최신 언어 모델을 활용하여 YouTube 동영상 대본에서 검색 가능한 데이터베이스를 만들고, FAISS 라이브러리를 사용하여 유사성 검색 쿼리를 수행하고, 관련성 있고 정확한 정보로 사용자 질문에 응답하는 방법을 보여줍니다.

LangChain은 언어 모델로 구동되는 애플리케이션을 개발하기 위해 설계된 포괄적인 프레임워크입니다. 가장 진보되고 차별화된 애플리케이션은 데이터를 인식하고 에이전트화하여 언어 모델이 다른 데이터 소스와 연결하고 해당 환경과 상호 작용할 수 있도록 지원하기 때문에 단순히 API를 통해 LLM을 호출하는 것 이상의 기능을 제공합니다. LangChain 프레임워크는 이러한 원칙을 해결하기 위해 특별히 구축되었습니다.

This repository focuses on experimenting with the LangChain library for building powerful applications with large language models (LLMs). By leveraging state-of-the-art language models like OpenAI's GPT-3.5 Turbo (and soon GPT-4), this project showcases how to create a searchable database from a YouTube video transcript, perform similarity search queries using the FAISS library, and respond to user questions with relevant and precise information.

LangChain is a comprehensive framework designed for developing applications powered by language models. It goes beyond merely calling an LLM via an API, as the most advanced and differentiated applications are also data-aware and agentic, enabling language models to connect with other data sources and interact with their environment. The LangChain framework is specifically built to address these principles.

## LangChain

The Python-specific portion of LangChain's documentation covers several main modules, each providing examples, how-to guides, reference docs, and conceptual guides. These modules include:

1. Models: Various model types and model integrations supported by LangChain.
3. Prompts: Prompt management, optimization, and serialization.
3. Memory: State persistence between chain or agent calls, including a standard memory interface, memory implementations, and examples of chains and agents utilizing memory.
4. Indexes: Combining LLMs with custom text data to enhance their capabilities.
5. Chains: Sequences of calls, either to an LLM or a different utility, with a standard interface, integrations, and end-to-end chain examples.
6. Agents: LLMs that make decisions about actions, observe the results, and repeat the process until completion, with a standard interface, agent selection, and end-to-end agent examples.

## Use Cases
With LangChain, developers can create various applications, such as customer support chatbots, automated content generators, data analysis tools, and intelligent search engines. These applications can help businesses streamline their workflows, reduce manual labor, and improve customer experiences.

## Service
By selling LangChain-based applications as a service to businesses, you can provide tailored solutions to meet their specific needs. For instance, companies can benefit from customizable chatbots that handle customer inquiries, personalized content creation tools for marketing, or internal data analysis systems that harness the power of LLMs to extract valuable insights. The possibilities are vast, and LangChain's flexible framework makes it the ideal choice for developing and deploying advanced language model applications in diverse industries.

## Requirements

- [Python 3.6 or higher](https://www.python.org/downloads/)
- [LangChain library](https://python.langchain.com/en/latest/index.html)
- [OpenAI API key](https://platform.openai.com/)
- [SerpAPI API Key](https://serpapi.com/)

## OpenAI API Models
The OpenAI API is powered by a diverse set of [models](https://platform.openai.com/docs/models) with different capabilities and price points. You can also make limited customizations to our original base models for your specific use case with fine-tuning.

## Installation

#### 1. Clone the repository

```bash
git clone https://github.com/your-username/langchain-experiments.git
```

#### 2. Create a Python environment

Python 3.6 or higher using `venv` or `conda`. Using `venv`:

``` bash
cd langchain-experiments
python3 -m venv env
source env/bin/activate
```

Using `conda`:
``` bash
cd langchain-experiments
conda create -n langchain-env python=3.8
conda activate langchain-env
```

#### 3. Install the required dependencies
``` bash
pip install -r requirements.txt
```

#### 4. Set up the keys in a .env file

First, create a `.env` file in the root directory of the project. Inside the file, add your OpenAI API key:

```makefile
OPENAI_API_KEY=your_api_key_here
```

Save the file and close it. In your Python script or Jupyter notebook, load the `.env` file using the following code:
```python
from dotenv import load_dotenv, find_dotenv
load_dotenv(find_dotenv())
```

By using the right naming convention for the environment variable, you don't have to manually store the key in a separate variable and pass it to the function. The library or package that requires the API key will automatically recognize the `OPENAI_API_KEY` environment variable and use its value.

When needed, you can access the `OPENAI_API_KEY` as an environment variable:
```python
import os
api_key = os.environ['OPENAI_API_KEY']
```

Now your Python environment is set up, and you can proceed with running the experiments.

## Datalumina

This document is provided to you by Datalumina. We help data analysts, engineers, and scientists launch and scale a successful freelance business — $100k+ /year, fun projects, happy clients. If you want to learn more about what we do, you can visit our [website](https://www.datalumina.io/) and subscribe to our [newsletter](https://www.datalumina.io/newsletter). Feel free to share this document with your data friends and colleagues.

## Tutorials
For video tutorials on how to use the LangChain library and run experiments, visit the YouTube channel: [youtube.com/@daveebbelaar](youtube.com/@daveebbelaar)

