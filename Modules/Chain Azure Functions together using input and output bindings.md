# Knowledge check
Although this is not intended to be an exhaustive list, the following are some resources related to the topics covered in this module that you might find interesting:

* Azure Functions documentation
* Azure Serverless Computing Cookbook
* How to use Queue storage from Node.js
* Introduction to Azure Cosmos DB: SQL API
* A technical overview of Azure Cosmos DB
* Azure Cosmos DB documentation

## Check your knowledge

1. Which of the following is an advantage of using bindings in your Azure Functions to access data sources and data sinks?
    - [ ] They provide access to more data sources than are available using code.
    - [ ] They let you connect to Azure resources without authentication.
    - [x] They simplify the connection process; you don't need to code specific connection logic.

Answer: Bindings provide a declarative way to connect to data. They let you avoid the complexity of coding connection logic like making a database connection or invoking web API interfaces.

2. What is the name of the file that contains function configuration data?

    - [ ] config.txt
    - [ ] config.json
    - [x] function.json

Answer: The configuration is named function.json, which contains JSON configuration data such as binding declarations.

3. How many triggers must a function have?

    - [ ] Zero
    - [x] One
    - [ ] Two

Answer: A function must have exactly one trigger.