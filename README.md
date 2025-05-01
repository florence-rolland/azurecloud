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
1. Automated release
We want to trigger a release pipeline using Azure cli. 

Before running the pipeline, it is necessary to be logged. 
For that purpose, if we use token-based authentication, we can run a command like
`echo  $aztoken | az devops login --organization https://dev.azure.com/iointeractive/`

The command starts with: `az pipelines release create`

What is your approach? You allowed to browse code on GitHub.com, use the Internet etc. 
Comment on what you are looking for, what the code means. 
We are looking for an approach, not runable code. 

2. Let us talk about authentication
The classic type of authentication is token-based authentication. 
What kind of challenges / issues / security concerns would that pose (assuming a self-hosted Windows agent). 
What are the alternatives?

Hint: 
MS documentation with supported options
https://learn.microsoft.com/en-us/azure/devops/pipelines/agents/agent-authentication-options?view=azure-devops

