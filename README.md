# 🤖 AI Email Agent with Gemma 3n E4B

This repository contains a Google Colab notebook that creates an automated email agent. The agent is designed to intelligently generate and send personalized emails for professional outreach, such as job applications or networking.

The core of the agent's functionality is a pipeline that:

1. # **Scrapes company information** from websites to find key details and potential email addresses.

2. **Generates a personalized email** using the powerful **Gemma 3n E4B** large language model from Google via the Hugging Face library.

3. **Sends the email** using the Gmail API.

## ✨ Features

* ✅ **Automated Company Scraping:** Efficiently extracts company descriptions and email addresses from target websites.

* ✅ **AI-Powered Personalization:** Leverages Gemma 3n E4B to craft unique, context-aware emails that highlight relevant skills and projects.

* ✅ **Gmail API Integration:** Securely sends emails directly from your Gmail account.

* ✅ **Ethical Scraping:** Includes built-in rate limiting and a respectful approach to web scraping.

* ✅ **Colab-Ready:** Designed to run seamlessly in a Google Colab environment, with support for GPU acceleration.

## 📦 Installation and Setup

### Prerequisites

* A Google account to run the notebook in Google Colab.

* A Hugging Face account with a user access token.

* A Gmail account with API access enabled (follow the Google Developers documentation to set up OAuth2 credentials).

### Steps

1. Open the `Email-Agent-Updated.ipynb` notebook in Google Colab.

2. Go to **Runtime > Change runtime type** and ensure that a GPU is selected.

3. Add your Hugging Face user access token as a secret in Colab. Go to the "Secrets" tab (lock icon) on the left sidebar, click **+ New secret**, and add a secret with the name `HF_TOKEN` and your token as the value.

4. Run the installation and setup cells at the beginning of the notebook (`!pip install ...`).

5. In the `API Key Setup` section, the notebook will use your `HF_TOKEN` to authenticate with Hugging Face.

6. Follow the instructions in the notebook to authenticate with your Gmail account.

7. Fill in your personal profile details in the `Personal Profile Setup` section.

8. Define your target companies and their URLs in the `Target Companies Setup` section.

9. Run the main agent cells to generate and, optionally, send the personalized emails.

## ⚙️ Project Structure

* `Email-Agent-Updated.ipynb`: The main Colab notebook containing all the code and instructions.

* `README.md`: This file, providing an overview of the project.

* `requirements.txt`: A list of all Python libraries needed to run the notebook.

## 📜 Ethical Considerations

This tool is designed for professional and ethical use. Please use it responsibly and in accordance with the terms of service of the websites and APIs you interact with. Avoid excessive scraping and respect rate limits.
