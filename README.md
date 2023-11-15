# watsonx-rag

This notebook provides a sample pipeline combining RAG with LLMs.

To use watsonx.ai LLM in IBM Cloud you will need to [Sign Up](https://www.ibm.com/docs/en/watsonx-as-a-service?topic=getting-started) for an account to retrieve the required credentials.

## Setup

This notebook was tested using Python 3.11.

`pip3 install requests chromadb pypdf httpx ibm-watson-machine-learning sentence-transformers`

If you set up an account you will need to populate an `.env` file based on your environment:

```
API_KEY=<your-ibm-cloud-api-key>
IBM_CLOUD_URL=https://us-south.ml.cloud.ibm.com
PROJECT_ID=<your-project-id>
```

> **_NOTE:_**  If you work in the Frankfurt instance use `eu-de` insead of `us-south` (Dallas) for the IBM Cloud URL

Finally, place a sample PDF file into the `db_files` folder that will be used for indexing.

