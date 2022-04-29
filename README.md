# azuresetup

This repo includes an Ansible Automation Platform (AAP) playbook to quickly poplulate an instance of AAP with some sample content to be used in an Azure Cloud environment.


**Instructions**

- Add the Azure credentials to your AAP instance and give it the following name: **'Microsoft Azure Resource Manager'**
-- The credential type is also called 'Microsoft Azure Resource Manager'
-- You will need to provied the Subscription ID, Tenant ID, Client ID (App ID), and Client Secret (App Secret)

- Add the Ansible Automation Platform credentials to your AAP instance and give it the following name: **'This AAPs Credentials'**
  - The credential type is called 'Red Hat Ansible Automation Platform'
  - You will need to provied the admin user and password, or the OAuth token

- Create a project and name it 'setup project'
  - For the **Source Control Credential Type** select **Git** from the dropdown
  - For the **Source Control URL** enter the following:  https://github.com/HichamMourad/azuresetup.git

- Create a Template (Add Job Template) and name it 'setup template'
  - For the **Inventory** select **Demo Inventory**
  - For the **Project** select **setup project**
  - For the **Playbook** select **azuresetup.yml**
  - For the **Credentials** select **This AAPs Credentials**
  - Save and launch this template.  Once complete you will find a number templates you can leverage, and there's also a Workflow Template.

Please customize any Extra Vars as needed for your environmnet.
Enjoy this sample content.
