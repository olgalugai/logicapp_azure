# ARM template to deploy Logic App connected to the storage account

File template.json is used to deploy:
- One storage account
- Two blob containers (test1, test2)
- API connection to the storage account
- Logic App

# Logic App identifies the files older than 30 minutes in each container and deletes it.

An app is set to run every day which can be changed in Recurrence section of the workflow block.

The time and date of the files to be deleted can be modified in "Filter_array" in type "Query" in "where" formula.

# Deployment

Custom deployment in Azure Portal or using Powershell or Azure CLI. The parameters for the deployment are included in template.json. They can be put in a separate parameters.json file.

Enter your subscription id in the gap of the path below the comment.

Created to practice Logic Apps deployment.