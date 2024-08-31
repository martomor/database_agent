# Building Your Own Database Agent


This repository contains my notes and code for the [Building Your Own Database Agent](https://www.deeplearning.ai/short-courses/building-your-own-database-agent/) offered by DeepLearning AI.

***Note:*** Please note that I have changed some of the code from calling Azure OpenAI endpoints to calling OpenAI directly, as I don’t have Azure OpenAI available:

- Notebooks L2 and L3 are calling OpenAI
- Notebooks L4 and L5 are calling AzureOpenAI

## Langchain Data Agents Summary

- **Natural Language to SQL Translation:** 
  Leverage Azure OpenAI and LangChain to create agents that convert user inputs into executable SQL queries.

- **LangChain Orchestration:**
  Implement LangChain to manage agent workflows and enable seamless database interactions based on natural language commands.

- **Function Calling for Enhanced Efficiency and Security:**
  Use Azure OpenAI’s function calling capability to send optimized and secure SQL queries, improving agent performance and safeguarding data operations.

- **Assistants API Integration:**
  Integrate with the Assistants API to streamline database connections, allowing you to create custom agents that efficiently handle database queries.


**Data Base Agents:**

![General Overview Agents](assets/general_overview_agents.png)

## How to use this repo

To get started, please follow the instructions below:

1. Clone the repository to your local machine:
```
git clone https://github.com/martomor/database_agent.git
```

2. Install Python 3.11.9 on your system. You can use either pyenv or conda to manage your Python versions. Here are the steps for each option:

    - Using pyenv:
      - Install pyenv by following the instructions [here](https://github.com/pyenv/pyenv#installation).
      - Once pyenv is installed, run the following command to install Python 3.11.9:
         ```
         pyenv install 3.11.9
         ```
      - Set Python 3.11.9 as the global version by running:
         ```
         pyenv global 3.11.9
         ```

    - Using conda:
      - Install conda by following the instructions [here](https://docs.conda.io/projects/conda/en/latest/user-guide/install/index.html).
      - Create a new conda environment with Python 3.11.9 by running:
         ```
         conda create -n dbagent python=3.11.9
         ```
      - Activate the environment by running:
         ```
         conda activate dbagent
         ```

3. Install the required dependencies using either pip or Poetry. Here are the steps for each option:

    - Using pip:
      - Navigate to the project directory:
         ```
         cd database_agent
         ```
      - Install the dependencies:
         ```
         pip install -r requirements.txt
         ```

    - Using Poetry:
      - Navigate to the project directory:
         ```
         cd database_agent
         ```
      - Install Poetry by following the instructions [here](https://python-poetry.org/docs/#installation).
      - Install the dependencies:
         ```
         poetry install
         ```

