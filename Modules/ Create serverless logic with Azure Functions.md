# Summary

You've learned how to use Azure Functions to host business logic services in the cloud. It's a great way to add hosted services to your solution that can scale and grow with your business. You focus on the code using the language of your choice, and Azure manages the infrastructure. Functions can integrate with other services, like Event Grid, GitHub, Twilio, Microsoft Graph, and Logic Apps to create complex and robust serverless workflows quickly and easily.

# Clean up
The sandbox automatically cleans up your resources when you're finished with this module.

When you're working in your own subscription, it's a good idea at the end of a project to identify whether you still need the resources you created. Resources left running can cost you money. You can delete resources individually or delete the resource group to delete the entire set of resources.

# Check your knowledge
1. Which of the following best defines serverless logic?
    - [ ] Code you write that doesn't run on servers.
    - [ ] Code you write that runs on servers you manage.
    - [x] Code you write that runs on servers a cloud provider manages.

Answer: Serverless doesn't mean there are no servers - it just means the developer doesn't have to worry about servers. Instead, a cloud provider such as Azure, manages servers.

2. The container that groups functions into a logical unit for easier management, deployment, and sharing of resources is called?
    - [ ] Resource group
    - [x] Function app
    - [ ] Function collection

Answer: A function app is a way to organize and collectively manage your functions. A function app is comprised of one or more individual functions that are managed together by Azure App Service. All the functions in a function app share the same pricing plan, continuous deployment, and runtime version.

3. We secured our function against unknown HTTP callers by requiring a function-specific API key be passed with each call. Which of the following fields is the name header in the HTTP requests that needs to contain this key?
    - [x] x-functions-key
    - [ ] x-requested-with
    - [ ] x-csrf-token

Answer: The API can be included in a query string variable named "code", or it can be included in an x-functions-key HTTP header.