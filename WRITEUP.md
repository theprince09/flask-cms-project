Azure Deployment Write-up
Resource Choice Analysis
This project required deploying a Flask-based CMS application to Azure. Two deployment options were considered: Virtual Machines (IaaS) and Azure App Service (PaaS).

Cost
Virtual Machines require paying for compute resources even when the application is idle. Azure App Service offers a Free F1 tier, which is sufficient for small projects like this CMS application. Therefore, App Service is more cost-effective.

Scalability
Virtual Machines require manual scaling and load balancing. Azure App Service provides built-in scaling features and automatic infrastructure management.

Availability
Azure App Service includes built-in load balancing and high availability features managed by Azure. With Virtual Machines, the developer must configure availability sets and load balancers manually.

Workflow
Deploying to a Virtual Machine requires configuring the OS, installing dependencies, and managing server updates. Azure App Service simplifies deployment through GitHub integration and automatic builds.

Deployment Decision
Azure App Service was selected for deploying the Flask CMS application. It provides easier deployment, reduced infrastructure management, and cost savings. Since the project is a small web application, the free tier of App Service is sufficient.

When Virtual Machines Might Be Preferred
If the application required full control of the operating system, custom networking, or specialized software dependencies, a Virtual Machine would be a better option. Applications requiring deep infrastructure customization or complex server configurations might benefit from using a VM.
