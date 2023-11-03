# azure_flask_deployment

### Assignment
- Course: HHA 504
- Homework assignment #2: Introduction to Flask and Azure deployment

### Summary of my assignment
- Created a Flask application locally on Cloud Shell.
- Deployed the Flask application using Azure App Service.
- Flask application link: **beckie-504-flask.azurewebsites.net**

### Steps to replicate my assignment
#### 1. Create a Flask application on Cloud Shell:
- Create a new Github repository named `azure_flask_deployment` in your Github account. Include a README.md file.
- Copy the Github repository as a URL under `<> Code`.
- In your Cloud Shell terminal, type `git clone` and paste the URL. This will create a clone of the Github repository locally in your Cloud Shell.
- In your Cloud Shell environment, create a python file named `app.py`. You can copy the code from [here](https://github.com/Beczheng/azure_flask_deployment/blob/main/app.py) and paste it into your file.
- Create a text file named `requirements.txt`. You can copy the code from [here](https://github.com/Beczheng/azure_flask_deployment/blob/main/requirements.txt) and paste it into your file.
- Create the following HTML files: `base.html`, `about.html`, and `random.html`. You can copy the codes from [here](https://github.com/Beczheng/azure_flask_deployment/tree/main/templates) and paste them into your files.
- Create a folder named `templates` and put all of the HTML files in it.
- In your Cloud Shell terminal, add the changes by typing `git add`.
- In your Cloud Shell terminal, commit the changes by typing `git commit -m 'insert a message'`.
- In your Cloud Shell terminal, push the changes by typing `git push`. This will push the changes to the repository in your Github account.

#### 2. Deploy the Flask application using Azure App Service:
- In your Cloud Shell terminal, type `curl -sL https://aka.ms/InstallAzureCLIDeb | sudo bash`. This will install the Azure CLI.
- Type `az` to check if Azure CLI is installed.
- Type `az login --use-device-code`. A link with a code will appear. Click on the link and enter the code. Then, login to your Microsoft Azure account. This will give Cloud Shell permission to access your Azure account.
- Type `az account list --output table`. Make sure that you are using the correct subscription. If not, type `az account set --subscription <SubscriptionId>` to change it.
- Type `az group list` to double check everything.
- Type `az webapp up --name <appname> --runtime PYTHON:3.9 --sku B1`. This will create a webapp for your Flask app.

#### 3. Locate the link to the Flask application: 
- In your Microsoft Azure account, search and click on "App Services".
- Click on the name of your webapp.
- Click on the link to your webapp under "default domain".






