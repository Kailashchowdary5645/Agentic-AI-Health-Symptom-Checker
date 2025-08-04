🚀 Getting Started
1. Clone the Repository

git clone https://github.com/your-username/agentic-ai-health-symptom-checker.git
cd agentic-ai-health-symptom-checker

2. Install Dependencies
For Python:

pip install -r requirements.txt

For Node.js:

npm install

3. Configure IBM Services
Create an IBM Cloud Lite account.
Set up Watsonx Assistant, Language Translator, Watson Discovery, and Cloudant.
Add credentials in a .env file:

ASSISTANT_API_KEY=your-api-key
TRANSLATOR_API_KEY=your-api-key
DISCOVERY_API_KEY=your-api-key

4. Run Locally
For Python:

python app.py

For Node.js:

npm start


✅ Key Requirements for It to Work
1. IBM Cloud Account

Ensure you have an IBM Cloud Lite account with access to Watsonx and Watson Machine Learning services.

2. API Key Configuration
Enter your IBM Cloud API key when prompted:

api_key = getpass.getpass("Please enter your api key (hit enter): ")

3. Space and Project IDs
Replace:

space_id = "47d05434-ab7b-4838-8163-e80e6ded0c19"
source_project_id = "3558480f-f5a0-4ef2-ae91-e11cd9bb4007"

with your actual IBM Cloud space ID and project ID.

4. Model ID
This code uses meta-llama/llama-3-3-70b-instruct from watsonx.ai. Make sure it is available in your region and project.

5. Run in Watson Studio or Jupyter
This notebook is designed for IBM Watson Studio or any Jupyter environment with ibm-watsonx-ai and langchain_ibm installed.

6. Install Required Libraries

pip install ibm-watsonx-ai langchain_ibm

7. AI Service Deployment

The notebook walks through:

Function definition (gen_ai_service)

Local testing

Deployment to Watsonx space

REST API testing