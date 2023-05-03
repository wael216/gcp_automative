# gcp_ai_log_analyzer

## Description
Set up the required APIs and SDKs:

Enable the necessary GCP APIs, such as Compute Engine, Cloud Functions, Cloud Build, and Cloud Storage, in your GCP project.
Install and initialize the Google Cloud SDK on your local machine.
Obtain an API key from OpenAI to access the ChatGPT API.
Create a Cloud Function to handle user requests and interact with GCP service with gcp_function.py

Deploy the Cloud Function:

Create a requirements.txt file with the dependencies in the file

Deploy the function using the Google Cloud CLI:
```
gcloud functions deploy chatbot \
    --runtime python310 \
    --trigger-http \
    --allow-unauthenticated \
    --set-env-vars OPENAI_API_KEY=<YOUR_OPENAI_API_KEY>
```

Create a chatbot interface with index.html
