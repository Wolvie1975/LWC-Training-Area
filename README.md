Salesforce LWC Development Environment with Codespaces
This repository provides a ready-to-use template for developing Salesforce Lightning Web Components (LWC) in a GitHub Codespace.

How to Use This Template
Click the "Use this template" button on GitHub to create your own repository from this template.

Once your repository is created, click the "Code" button and select "Create a new codespace".

GitHub will build your cloud-based development environment. This may take a few minutes the first time.

Developing LWC
1. Authorize an Org
Once your Codespace is running, you need to connect it to a Salesforce org.

Open the Command Palette (Ctrl+Shift+P or Cmd+Shift+P).

Run the command: SFDX: Authorize an Org.

Follow the prompts. Choose a login URL (e.g., Production or Sandbox) and provide an alias for your org.

A new browser tab will open for you to log in to Salesforce. After logging in, grant access to the Salesforce CLI.

2. Run the LWC Local Development Server
To see your components locally without deploying them:

Open the terminal in your Codespace.

Run the following command:

sf lwc start

The server will start, and Codespaces will prompt you to open the URL in a new browser tab. You can now see and interact with your helloWorld component live! Any changes you save to the code will be reflected instantly.

3. Deploying to Your Org
When you are ready to deploy your components to the Salesforce org you authorized:

Right-click on the force-app/main/default directory.

Select SFDX: Deploy Source to Org.