# Azure-devops-pipeline-Secure-file
Automating Secure File Uploads and Deletions in Azure Pipelines Using Bash Scripting

1. **secureFileName:** Specifies the name of the secure file to be uploaded (e.g., "Info.plist").
2. **personalAccessToken:** Represents the Personal Access Token (PAT) used for authentication with Azure DevOps.
3. **azureDevOpsOrganization:** Refers to the name of the Azure DevOps organization where the project resides.
4. **azureDevOpsProjectID:** Denotes the unique ID of the Azure DevOps project where the secure file will be uploaded.
5. **secureFilePath:** Points to the local file path of the secure file "Info.plist" that needs to be uploaded

**1. Script Functionality:**
- Variable Definition: The script prompts the user to provide the required variables or accepts them as command-line arguments.
- Secure File Upload: It utilizes the Azure DevOps REST API with curl commands to perform the following actions:
- Checks for existing files with the same name.
- Deletes existing files if necessary (optional).
- Uploads the specified local file as a secure file in the designated project.
