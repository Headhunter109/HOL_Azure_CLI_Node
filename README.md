# Material for Azure x-plat CLI and Node SDK Hands On Lab
**Work In Progress**

## Prerequisite

* Azure Subscription
    * If you don't have it, please see [the page](https://azure.microsoft.com/en-us/pricing/free-trial/) to get free one-month trial credits.
    
* Your Client
    * Mac OS X or Windows
    * Node.js and npm - [Downloads](https://nodejs.org/en/download/)
    * SSH Client
    * Git
    
## Part 1 - Install Azure x-plat  CLI
**do not use OS-specific installer packages, but use npm**

Check if node and npm were installed properly by opening a Command or Terminal window and typing

    npm -v

Use the following command to install the Azure CLI:

    npm install azure-cli -g

Once the Azure CLI has been installed, you will be able to run the azure command from your command-line user interface (Bash, Terminal, Command prompt, and so on). For example, to run the help command, type the following:

    azure help
    
References:
*  [Install the Azure CLI](https://azure.microsoft.com/en-us/documentation/articles/xplat-cli-install/)

## Connect to Azure
Interactively logging in is easy: type azure login and follow the prompts as shown below:

    azure login                                                                                    
    info:    Executing command login
    info:    To sign in, use a web browser to open the page http://aka.ms/devicelogin. Enter the code XXXXXXXXX to authenticate. If you're signing in as an Azure AD application, use the --username and --password parameters.
    
Copy the code offered to you, above, and open a browser to http://aka.ms/devicelogin. Enter the code, and then you are prompted to enter the username and password for the identity you want to use.

Your account may have more than one subscription. You can list your subscriptions by typing:

    azure account list

You can set the current Azure subscription by typing the following. Use the subscription name or the ID that has the resources you want to manage.

    azure account set <subscription name or ID>

By default, the Azure CLI starts in the service management mode (asm mode). Type the following to switch to resource group mode.

    azure config mode arm

References:
* [Connect to an Azure subscription from the Azure Command-Line Interface (Azure CLI)](https://azure.microsoft.com/en-us/documentation/articles/xplat-cli-connect/#use-the-log-in-method)

## 

References:
* [Deploy and manage virtual machines by using Azure Resource Manager templates and the Azure CLI](https://azure.microsoft.com/en-us/documentation/articles/virtual-machines-deploy-rmtemplates-azure-cli/)