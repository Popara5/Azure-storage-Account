# Azure-storage-Account
Create a new container inside the Storage 
Step-by-Step Guide to Create an Azure Storage Account and a Container
Step 1: Log in to Azure Portal
Go to Azure Portal.

Sign in with your credentials.

Step 2: Create a Storage Account
Click on "Create a resource" in the left menu.

Search for "Storage Account" and select it.

Click "Create".

Fill in the required details:

Subscription: Select your Azure subscription.

Resource Group: Create a new one or use an existing one.

Storage Account Name: Enter a unique name (e.g., mystorageaccount123).

Region: Choose a location near you.

Performance: Standard (for most use cases) or Premium (for high performance).

Redundancy: Select an option (e.g., Locally-redundant storage (LRS)).

Click "Review + Create", then "Create".

Step 3: Create a Container in the Storage Account
Once the storage account is deployed, go to Storage Accounts and select your newly created storage account.

In the left menu, under Data storage, click on "Containers".

Click "+ Container".

Enter a name for your container (e.g., mycontainer). Container name do not have to be globally unique as storage account. You can use dashes in the container name if you want to as well. "my-container" Remember to enable anonymous access to object because we did disabled public anonymoue access at the account level. 

Choose the public access level (Private, Blob, or Container).

Click "Create".

