# Milestone 4
The Lodging API is now complete! All it needs is a CI/CD pipeline to facilitate integrating future features that could be added to it!

## Goal
Your goal as a developer is to come up with a working pipeline that:
1. Builds the given solution
2. Tests it
3. Runs a code analysis on the solution
4. Deploys the webapp to the world wide web

### Setting up in Azure DevOps
1. Create a new project in Azure DevOps
2. Add the working solution to the Azure Repo associated with the project
3. Start building the pipeline

### Setting up Sonar Cloud
1. Create a project manually in Sonar Cloud
2. Go to your account settings, in the security tab, generate a token
3. In the project containing your pipeline, in project settings, navigate to service connections, under pipelines
4. Add new connection, select sonar cloud
5. Use the generated token to connect your pipeline to sonar cloud

### Setting up an App Service in Azure
1. Go to the services portal in azure
2. Select the app services option
3. Create a new app service, make sure to select the free options

### Remarks 
- Note that you don't need to edit the given solution in any way. You only need to create the pipeline.
- Use Azure Devops to create the pipeline

### Hint
A sample pipeline.yml file has been provided to base your pipeline on. This sample pipeline is still incomplete (and unusable)!

## Files
### pipeline.yml
Sample pipeline that builds the application. 

### creds.txt
This is where you put in your pipeline credentials. First line must be the organization, second line the project, and the third line will be the definition id of your pipeline.

### .gitignore
This is essential when uploading your files to the Azure Repo, this makes sure only the solution source code gets uploaded