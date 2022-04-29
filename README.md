# azuresetup

This repo includes an Ansible Automation Platform (AAP) playbook to quickly poplulate an instance of AAP with some sample content to be used in an Azure Cloud environment.


**Instructions

- Add the Azure credentials to your AAP instance and give it the following name: **'Microsoft Azure Resource Manager'**
-- The credential type is also called 'Microsoft Azure Resource Manager'
-- You will need to provied the Subscription ID, Tenant ID, Client ID (App ID), and Client Secret (App Secret)

- Add the Ansible Automation Platform credentials to your AAP instance and give it the following name: **'This AAPs Credentials'**
-- The credential type is called 'Red Hat Ansible Automation Platform'
-- You will need to provied the admin user and password, or the OAuth token

- Create a project and name it 'setup project'
-- For the **Source Control URL** enter the following:  
