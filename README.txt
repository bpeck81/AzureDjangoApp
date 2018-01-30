# AzureDjangoApp
Deploy a blank Python Django Web App to Azure

Steps:

GET AZURE ACCESS
1. Create Dreamspark account on Microsoft Imagine Website
2. Verify student status to gain azure access
3. Login to Azure Portal
4. Press New -> Web App
    1. Enter an app name
    2. If required, create a new resource group; Just type in a name relevant to you app resources
    3. If required, create a new app service plan; Just follow the steps on screen
    4. Select “Create” at the bottom
5. Select created web app on dashboard
6. Select Deployment options -> Choose Source -> Local Git Repository
    1. If required, create user by entering username and password
7. Select OK to finish deployment setup
8. Select Properties on the left panel and scroll to the GIT URL. Copy the url.

CREATE LOCAL REPOSITORY
1. Run in Terminal
    1. git clone https://github.com/bpeck81/AzureDjangoApp.git
    2. cd AzureDjangoApp
    3. git remote add azure <copied git url>
    4. git push azure master
    5. <enter Azure user password>
2. Return to Azure Overview tab and press browse to view the deployed site!

NOTE
If you want to deploy an existing Django project to Azure add the following files from the repository to your project and follow the deployment steps above:
	requirements.txt,
	web.config,
	ptvs_virtualenv_proxy.py

CREDITS
https://github.com/Azure-Samples/app-service-web-python-get-started
