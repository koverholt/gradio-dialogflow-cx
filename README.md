# gradio-dialogflow-cx

A Python notebook that integrates Gradio (app frontend) with Dialogflow CX
(conversational backend)

![Screenshot of a Gradio app integrated with Dialogflow CX](/images/chatbot.png)

## Prerequisites

- You have a Google Cloud account
- You have enabled the Dialogflow CX APIs in Google Cloud
- You've created a virtual agent (try using one of the pre-built agents!)

## Usage

1. Clone this repo and `cd` into this directory
2. Install dependencies with
   ```
   pip install -r requirements.txt
   ```
3. Open the notebook
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
6. View the app in your browser on your local machine
7. (Optional) Make your Gradio app link publicly accessible by running a new
   cell with `demo.launch(share=True)`
