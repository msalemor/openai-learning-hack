# openai-learning-hack

## Demo environment

This demo runs on .NET interactive on VS Code using the polyglot extension. Basically, it is a Jupyter notebook that runs C# instead of Python.

Recommended environment:

- Windows Subsystem for Linux (WSL) with Python 3 and .NET 6 o 7 installed
- VS Code
- Polyglot extension for VS Code

### OpenAI endpoint and keys

- The demo requires both GPT and ADA embedding enpoints
- Go to the Azure portal, go to the OpenAI service, and create endpoints for these two models
- Clone the repo
- Create a `notebooks\.env` file add the following variables or add environment variables instead:

```bash
GPT_OPENAI_KEY=<KEY>
GPT_OPENAI_DEPLOYMENT_NAME=<GPT_MODEL_NAME>
GPT_OPENAI_ENDPOINT=https://<NAME>.openai.azure.com/
GPT_OPENAI_FULL_ENDPOINT=https://<NAME>.openai.azure.com/openai/deployments/<GPT_MODEL_NAME>/chat/completions?api-version=2023-03-15-preview
OLD_GPT_OPENAI_FULL_ENDPOINT=https://<NAME>.openai.azure.com/openai/deployments/<GPT_MODEL_NAME>/chat/completions?api-version=2022-12-01

ADA_OPENAI_KEY=<KEY>
ADA_OPENAI_DEPLOYMENT_NAME=<ADA_MODEL_NAME>
ADA_OPENAI_ENDPOINT=https://<NAME>.openai.azure.com/
ADA_OPENAI_FULL_ENDPOINT=https://<NAME>.openai.azure.com/openai/deployments/<ADA_MODEL_NAME>/embeddings?api-version=2023-05-15
```

### Running the demo

- Open WSL, navigate to the `notebooks` folder
- To start VS Code type: `code .`
- Open the `notebooks\hack.ipynb` file
- At each cell, click the `play` button

