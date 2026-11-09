# 🚀 Social Media Post Creator 2.0

An AI-powered social media content creation automation built with **n8n and Google Gemini AI**.

Social Media Post Creator 2.0 helps simplify social media content creation by turning ideas and topics into engaging, ready-to-use social media posts using artificial intelligence.

This is an improved version of my original Social Media Post Creator, featuring an enhanced automation workflow and improved content creation experience.

> 🚧 **Project Status:** Automatic social media publishing is currently under construction and is not available yet. The current focus is on AI-powered content generation and post management.

## ✨ Features

- 🤖 **AI-Powered Content Generation:** Generate engaging social media content using Google Gemini AI.
- ✍️ **Automated Post Creation:** Turn your ideas and topics into ready-to-use social media posts.
- 👀 **Post Preview:** Review generated content before proceeding.
- ✅ **Human Approval:** Approve or reject generated posts before further processing.
- ⚡ **n8n Workflow Automation:** Automate the content creation process using n8n.
- 🔗 **Webhook Integration:** Connect the application with n8n through webhooks.
- 🚧 **Automatic Social Media Posting:** Under construction. Direct publishing to social media platforms is planned for a future update.

## 🛠️ Technologies Used

| Technology | Purpose |
|---|---|
| n8n | Workflow automation |
| Google Gemini AI | AI-powered content generation |
| Webhooks | Communication between application and n8n |
| API Integrations | Connecting external services |

## ⚙️ How It Works

The automation follows a simple workflow:

1. Enter a topic or idea for your social media post.
2. The application sends the request to the n8n webhook.
3. Google Gemini AI processes the topic and generates engaging content.
4. The generated post is returned to the application.
5. Preview and review the generated content.
6. Approve or reject the generated post.
7. Manage your content through the available workflow.

> **Coming Soon:** Automatic publishing directly to connected social media accounts.

## 📋 Requirements

Before setting up this automation, make sure you have:

- An n8n account (Cloud or self-hosted).
- A Google account.
- A Google Gemini API key.
- Access to the project source code.
- A web browser.

## 🔑 Step 1: Get Your Google Gemini API Key

Google Gemini AI is used to generate social media post content.

Follow these steps to generate your API key:

1. Visit [Google AI Studio](https://aistudio.google.com/).
2. Sign in using your Google account.
3. Navigate to the API Keys section.
4. Click **Create API Key**.
5. Select an existing Google Cloud project or create a new one if required.
6. Copy your newly generated API key.

**Direct Link:** https://aistudio.google.com/app/apikey

<details>
<summary>Important API Key Security Notes</summary>

- Never share your API key publicly.
- Never upload your API key to GitHub.
- Do not hardcode your API key into publicly accessible source code.
- Store your API credentials securely using n8n's credential management.
- Check your Google AI Studio account for API usage limits and applicable pricing.

</details>

## 🔗 Step 2: Set Up n8n

n8n is the automation platform responsible for connecting the application with Google Gemini AI.

1. Visit [n8n.io](https://n8n.io/).
2. Create an account or log in to your existing account.
3. Open your n8n workspace.
4. Import the provided workflow JSON file if included in this repository.
5. Open the imported workflow.
6. Review the nodes and their configurations.

You can use either:

- **n8n Cloud:** A hosted n8n environment.
- **Self-Hosted n8n:** Run n8n on your own server or local machine.

Official documentation: https://docs.n8n.io/

## 🔐 Step 3: Configure Google Gemini Credentials in n8n

After obtaining your Gemini API key, connect it to your n8n workflow.

1. Open your n8n workspace.
2. Open the Social Media Post Creator 2.0 workflow.
3. Locate the Google Gemini AI node.
4. Open its credential settings.
5. Create new Google Gemini credentials if required.
6. Paste your Gemini API key into the appropriate field.
7. Save your credentials.
8. Test the node to make sure the connection works.

**Note:** Make sure you select a Gemini model that is available to your API key and compatible with your workflow configuration.

## 🌐 Step 4: Configure the Webhook

The application communicates with n8n through a webhook endpoint.

Follow these steps:

1. Open your n8n workflow.
2. Select the Webhook node.
3. Open its configuration.
4. Copy the generated webhook URL.

n8n provides two types of webhook URLs:

| Webhook Type | Purpose |
|---|---|
| Test URL | Used during development and testing |
| Production URL | Used when the workflow is active |

Use the Test URL while developing and testing the automation.

Once everything is working correctly, activate your workflow and configure the Production URL in your application.

**Important:** Make sure your application is using the correct webhook URL.

## 🧪 Step 5: Test Your Automation

Before using the automation, test the complete workflow.

1. Open your n8n workflow.
2. Start listening for test webhook events if using the Test URL.
3. Open the application.
4. Enter a sample social media topic.
5. Submit the request.
6. Check whether the request reaches n8n.
7. Verify that Google Gemini generates the content.
8. Review the generated post in the application.
9. Test the available approval and rejection functionality.

If everything works correctly, your Social Media Post Creator 2.0 automation is ready to use.

## 🚧 Upcoming Features

Automatic social media publishing is currently under development.

Planned improvements include:

- Direct social media account integration.
- Automatic publishing of approved posts.
- Support for multiple social media platforms.
- Improved post scheduling and management.
- Additional content creation capabilities.

Stay tuned for future updates!

## 🐛 Troubleshooting

### 1. Gemini API Error

If Google Gemini is not generating content:

- Verify that your API key is correct.
- Check whether the selected Gemini model is available.
- Review your API usage and quota.
- Check the n8n execution logs for errors.

### 2. Webhook Not Responding

If your application cannot communicate with n8n:

- Verify your webhook URL.
- Make sure your workflow is active when using the Production URL.
- Make sure the Test URL is listening for requests during development.
- Check your n8n execution history.

### 3. Content Generation Not Working

If the generated content is not returned:

- Check your Gemini credentials.
- Review the Google Gemini node configuration.
- Inspect the n8n execution output.
- Verify that the incoming request contains the expected information.

### 4. Approval Functionality Not Working

- Verify the relevant workflow nodes.
- Check the webhook request and response configuration.
- Review the n8n execution logs.

## 🔒 Security

Security is important when working with APIs and automation workflows.

- Never commit API keys or private credentials to GitHub.
- Use n8n's credential management for sensitive information.
- Keep your webhook endpoints protected where appropriate.
- Avoid exposing private tokens in frontend code.
- Use appropriate authentication for production environments.

## 📚 Useful Resources

| Resource | Link |
|---|---|
| Google AI Studio | https://aistudio.google.com/ |
| Gemini API Key | https://aistudio.google.com/app/apikey |
| Gemini API Documentation | https://ai.google.dev/gemini-api/docs |
| n8n Official Website | https://n8n.io/ |
| n8n Documentation | https://docs.n8n.io/ |
| n8n Webhook Documentation | https://docs.n8n.io/integrations/builtin/core-nodes/n8n-nodes-base.webhook/ |

## 🤝 Contributing

Contributions, suggestions, and improvements are welcome!

If you find a bug or have an idea to improve this project, feel free to open an issue or submit a pull request.

## 📄 License

This project is open-source. Please check the repository's LICENSE file for licensing information.

## 👨‍💻 Author

**Ahmed Rabbani**

Independent n8n Automation Developer

- 🌐 Portfolio: https://ahmedautomates.netlify.app
- 💼 LinkedIn: https://www.linkedin.com/in/ahmed-rabbaniofficial/
- 🐙 GitHub: https://github.com/Ahmed-Rabban
- ▶️ YouTube: https://www.youtube.com/@Ahmed-Automates

---

⭐ **If you find this project useful, consider giving the repository a star!**

Built with ❤️ using n8n and Google Gemini AI.
