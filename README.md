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

Click on and open the conatiner once created, click on Upload, go ahead and add some objects to the container by browse files or simply drag and drop from one folder into the container. You can upload any file type up to about 4 TB in size into the container. You can uplad some loose files from your local Download directory and simply drag them over into the container. Once download into the container we have a text file, some image files, and we also have a few keynote as well. 
Choosing Advanced options to upload files into containers. In this case we are using a default block blob option
Blob types - Block blobs, Page blo,b and Append blob
Page blobs - are more for virtual hard drive files, and append blob are used for files that are continuously updated or appended too each other.   
Access Tier level can be set as Hot (preferred), Cool, cold, or Archive. 
Select upload after all of the files uploaded to the container. 
Click on the file uploaded into the container, first thing look at the URL link. Remmember that every individual file that you upload into a Blob container has its own unique URL assigned to it. 
If you want to view the entire URL click on the copy button, open up a new tap and paste it into there it will show the entire path. The structure of every path starts with https...storage account name, such as az900demo123, blob for a Blob container, .core.windows.net, and object name.   
And then after that, we have a slash in the container name, which is my-container. If we hit enter now the tab is an anonymous browsing tab, and we will not be able to access the file because that file has not been made public for anonymous access, which is why we are getting a piublic access is not permited error message once you hit enter. 

To enable public anonymous access to any file, which will actually enable anonymous access to all objects inside of my container, so we can go ahead and view it in a separate tab. 
To do that, we have to go back to the storage account settings ------> Easiest way to do that is to click on Storage accounts on the left hand top, then click on the account then from the right side of the page, if you scrow down a little bit further you will see the Blob anonymous access setting right there which current showing disabled. Go ahed and switch it to enabled that will switch the container to public access so we can go ahead and view the object in the new tab. 
Quick notice, you want to be very careful with the setting because you obviously do not want to put sensitive or customer data in a public storage account. 
Click on Disable and that will take to othe configuration settings, here choose to allow Blob anonymous access to enabled. 
Click on save  ----> the container has been set for anonymous access. 
Go back to the container to enable public anonymous access for all objects inside of it. 
 Data Storage ----> Containers ------> we will click on the containers from the left side once again, put a check next to the container named "my-container", and then click on the Change access level button, go ahead and click it, and we can choose to enable either anonymous reading access for only Blob files inside of the container or for the container itself. 

 Test it out by going to the tab with the error message, click on to the refresh button, and if we get it correctly we should see the immage file. And we have successfully enable public anonymous access to of our objects inside of that container, and we can now view that object in a new tab. 
 At this point, I have able to create a new container inside of our storage account, uploading some objects or files into that container, and then enabling public anonymous access so we can view the URL of that object in a new tab. 
 






