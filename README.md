# azure_flask_deployment
HHA 504: Week 2

Homework assignment #2: Introduction to Flask and Azure deployment

Summary
- Created a Flask application locally on Cloud Shell.
- Deployed the Flask application using Azure App Service.
- Flask application link: **beckie-504-flask.azurewebsites.net**

Steps
- Create a Flask application on Cloud Shell:
    1. Create a new Github repository named `azure_flask_deployment` in your Github account. Include a README.md file.
    2. Copy the Github repository as a URL under `<> Code`.
    3. In your Cloud Shell terminal, type `git clone` and paste the URL. This will create a clone of the Github repository locally in your Cloud Shell.
    4. In your Cloud Shell environment, create a python file named `app.py`. You can copy the code from [here](https://github.com/Beczheng/azure_flask_deployment/blob/main/app.py) and paste it into your file.
    5. Create a text file named `requirements.txt`. You can copy the code from [here](https://github.com/Beczheng/azure_flask_deployment/blob/main/requirements.txt) and paste it into your file.
    6. Create the following HTML files: `base.html`, `about.html`, and `random.html`. You can copy the codes from [here](https://github.com/Beczheng/azure_flask_deployment/tree/main/templates) and paste them into your files.
    7. Create a folder named `templates` and put all of the HTML files in it.
    8. In your Cloud Shell terminal, add the changes by typing `git add`.
    9. In your Cloud Shell terminal, commit the changes by typing `git commit -m 'insert a message'`.
    10. In your Cloud Shell terminal, push the changes by typing `git push`. This will push the changes to the repository in your Github account.

- Deploy the Flask application using Azure App Service:
    1. In your Cloud Shell terminal, type `curl -sL https://aka.ms/InstallAzureCLIDeb | sudo bash`. This will install the Azure CLI.
    2. Type `az` to check if Azure CLI is installed.
    3. Type `az login --use-device-code`. A link with a code will appear. Click on the link and enter the code. Then, login to your Microsoft Azure account. This will give Cloud Shell permission to access your Azure account. 
    3. Type `az webapp up --name <appname> --runtime PYTHON:3.9 --sku B1`. This will create a webapp for your Flask application.

- Locate the link to the Flask application: 
    1. In your Microsoft Azure account, search and click on "App Services".
    2. Click on the name of your webapp.
    3. Click on the link to your webapp under "default domain".






