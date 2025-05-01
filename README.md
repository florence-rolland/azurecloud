# azurecloud
Technical challenge for cloud build engineer

# resources
GHA to trigger ADO pipelines using GitHub actions
https://github.com/Azure/pipelines

Community repo with doc explaining how to trigger ADO pipelines with token-based authentication
https://github.com/JamesBurnside/jamesburnside.github.io/blob/51c36d3aa318692c799410dc962dba672bd61f56/posts/trigger-ado-pipeline-with-github-action.mdx#L2

Microsoft documentation for az pipelines cli
https://learn.microsoft.com/en-us/cli/azure/pipelines?view=azure-cli-latest

# exercise
We want to trigger a release pipeline using Azure cli. 

Before running the pipeline, it is necessary to be logged. 
For that purpose, if we use token-based authentication, we can run a command like
`echo  $aztoken | az devops login --organization https://dev.azure.com/iointeractive/`

The command starts with: `az pipelines release create`
