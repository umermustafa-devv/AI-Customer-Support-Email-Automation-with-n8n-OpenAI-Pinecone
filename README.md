# AI-Customer-Support-Email-Automation-with-n8n-OpenAI-Pinecone
![Image Alt Text](./image%20(1).png)
AI-powered customer support email automation using n8n, OpenAI, and Pinecone. This workflow automates the analysis of customer emails, categorizes them, and generates responses. Integrated with Gmail for email retrieval and Pinecone for vector storage, streamlining support operations.

## How to Run the Code

Follow these steps to set up and run the **AI Customer Support Email Automation** workflow locally.

### 1. Clone the Repository

First, clone the repository to your local machine:

git clone https://github.com/username/AI-Customer-Support-Email-Automation-with-n8n-OpenAI-and-Pinecone.git
cd AI-Customer-Support-Email-Automation-with-n8n-OpenAI-and-Pinecone

###  2. Install Prerequisites
Make sure you have Node.js installed. If not, download and install it from here.

Then, install n8n by running:
npm install n8n

###  3. Set Up API Credentials
You will need the following API keys:

Gmail OAuth2: Set up a Gmail API project in the Google Cloud Console. Enable Gmail API and create OAuth2 credentials. Save the credentials and authenticate in n8n.

OpenAI API Key: Get your OpenAI API key from OpenAI and add it to n8n.

Pinecone API Key: If using Pinecone for vector storage, sign up for Pinecone here and get the API key to set in n8n.

###  4. Configure n8n Workflow
Once all dependencies are installed and the API keys are configured:

Start n8n by running:
n8n

Access the n8n web interface by navigating to http://localhost:5678 in your browser.

Import the workflow from this repository into n8n by uploading the .json file that is part of this project.

###  5. Set Workflow Nodes in n8n
Gmail Trigger: Set up the Gmail trigger to automatically fetch new emails from your Gmail inbox.

Customer Support Evaluation: Configure the model to evaluate the email content and determine if it is related to customer support.

Response Generation: Use OpenAI's GPT-4 model to generate responses based on the email content.

Pinecone Vector Store: If you are using Pinecone, set up vector storage for storing customer support data for future reference and query optimization.

###  6. Test the Workflow
Once the workflow is set up:

Send a test email to the Gmail account connected to the workflow.

Ensure that the email is processed and a response is generated automatically based on the email content.

###  7. Deploy and Automate
For continuous operation, you can deploy the workflow to a cloud server or hosting platform like Heroku, AWS, or DigitalOcean.

You can also use PM2 or Docker to keep n8n running persistently in the background.

###  8. Monitor and Maintain
Monitor the system to ensure that emails are processed and that the generated responses are correct. Make sure to rotate your API keys regularly and maintain the workflow to ensure optimal performance.

