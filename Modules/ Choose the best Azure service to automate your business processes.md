# Knowledge check

## Scenario 1 - TV Adverts
You work for a company that makes TV adverts. You want to formalize two business processes:

* The advert review process. A completed advert is put through this editorial process to ensure that it meets the standards of taste, decency, grammar, style, and legal requirements in the jurisdiction where it will be broadcast.
The feedback collection process. A completed advert is also put through this process in which customers, the director, and members of the board of directors, can give feedback.
The advert review process should be managed by members of the creative team, because it will need to change regularly. The creative team would prefer not to have to wait for a developer to become available whenever a change is needed.

* The feedback collection process calls an on-premises SharePoint server. Because this server is not as reliable as a cloud-based server would be, developers want to carefully control the way the workflow retries this connection, if there is a failure.

## Scenario 2 - Camera Company Merger
You work for a company that makes digital cameras. The company has recently acquired a smaller company that makes lenses. You want to ensure that the same procedures are in use throughout the company for the following processes:

* Lens quality control. The company you acquired has a good reputation for lens reliability because of its quality control procedure. You want to implement this procedure across the merged company and integrate it with your parts ordering system, which includes a REST API.

* Ordering and dispatch. The company you acquired had no formal order and dispatch procedure, so you want to ensure its employees use your original business procedure. The ordering system has a user interface that is built as an Azure App service web app but you want to manage the order and dispatch workflow as a separate project.

You have hired a small team of developers to do the work and you prefer a design-first approach.


# Check your Knowledge
1. In the television advert company, which technology would you use for the advert review process?
    - [x] Microsoft Power Automate
    - [ ] Azure Logic Apps
    - [ ] Azure Functions
    - [ ] Azure App Service WebJobs

Answer: Azure WebJobs, Functions and Logic Apps don't permit the creative team, who are not developers, to manage the process. Instead use Microsoft Power Automate.

2. In the television advert company, which technology would you use for the feedback collection process?
    - [ ] Microsoft Power Automate
    - [ ] Azure Logic Apps
    - [ ] Azure Functions
    - [x] Azure App Service WebJobs

Answer: WebJobs are the only technology that permits developers to control retry policies.

3. In the merged camera company, which technology would you use for the lens quality control procedure?
    - [ ] Microsoft Power Automate
    - [x] Azure Logic Apps
    - [ ] Azure Functions
    - [ ] Azure App Service WebJobs

Answer: Azure Logic Apps is the only one of the four technologies that provides a design-first approach intended for developers.

4. In the merged camera company, which technology would you use for the ordering and dispatch procedure?
    - [ ] Microsoft Power Automate
    - [x] Azure Logic Apps
    - [ ] Azure Functions
    - [ ] Azure App Service WebJobs

Answer: Azure Logic Apps is the only one of the four technologies that provides a design-first approach intended for developers.