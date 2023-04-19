# Gradio app + Dialogflow CX agent

A Python notebook that integrates a
[Gradio chatbot app](https://gradio.app/docs/#chatbot) (frontend) with a
[Dialogflow CX virtual agent](https://cloud.google.com/dialogflow/cx/docs)
(conversational chatbot backend). Run
[this notebook](https://github.com/koverholt/gradio-dialogflow-cx/blob/main/notebook/gradio-dialogflow.ipynb)
and see for yourself!

<img src="/images/chatbot.png" width="600px" alt="Screenshot of a Gradio app integrated with Dialogflow CX">

## Prerequisites

- You have a
  [Google Cloud account](https://console.cloud.google.com/getting-started) and a
  [project](https://cloud.google.com/resource-manager/docs/creating-managing-projects)
- You have enabled the
  [Dialogflow CX API in Google Cloud](https://cloud.google.com/dialogflow/cx/docs/quick/setup#api)
  for your project
- You've created a
  [virtual agent](https://cloud.google.com/dialogflow/cx/docs/quick/build-agent)
  in Dialogflow CX (I suggest trying one of the
  [pre-built agents](https://cloud.google.com/dialogflow/cx/docs/concept/agents-prebuilt)!)

## Usage

1. Clone this repo and `cd` into this directory
2. Install dependencies with
   ```
   pip install -r requirements.txt
   ```
3. Open the
   [notebook in this repo](https://github.com/koverholt/gradio-dialogflow-cx/blob/main/notebook/gradio-dialogflow.ipynb)
4. Define the values in the notebook for your Google Cloud project ID,
   Dialogflow CX agent region, Dialogflow CX agent ID, and language. For
   example:
   ```
   PROJECT_ID = "my-awesome-google-cloud-project"
   LOCATION_ID = "global"
   AGENT_ID = "1111aa11-aaaa-1111-a111-1a1aa1a111aa"
   LANGUAGE_CODE = "en-us"
   ```
5. Run all of the cells in the notebook
6. View the app in your browser on your local machine and chat with it!
7. (Optional) Make your Gradio app link publicly accessible by running a new
   cell with `demo.launch(share=True)`
