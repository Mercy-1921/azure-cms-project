# Write-up
App Deployement using Microsoft Azure

## What Is Virtual Machine
An Azure Virtual Machine is part of Infrastructure as a Service (IaaS) in cloud computing. It provides complete control over the operating system and computing environment. Developers can run either Windows or Linux virtual machines and manage all configurations themselves. Virtual machines offer flexibility, scalability, and high availability, but they also require continuous maintenance such as system updates, security management, and software installation by the developer.

## What Is App Service
Azure App Service is a Platform as a Service (PaaS) offering that allows developers to focus on building and deploying applications without worrying about managing the underlying infrastructure. It is an HTTP-based platform used to host web applications, REST APIs, and mobile back-end services. Azure App Service supports multiple programming languages and integrates easily with continuous deployment tools.

### Appropriate solution
For deploying this web application, Azure App Service is the most suitable solution.

### Why I choose App service
-Azure App Service provides an integrated platform for building and hosting websites, web APIs, and mobile back-end services for different platforms and devices.
-Infrastructure tasks such as server maintenance, security patching, and scaling are handled automatically by Azure.
-It supports several programming languages including .NET, Java, Node.js, PHP, Ruby, and Python. Since this application is developed using Python, App Service is fully compatible.
-It allows fast deployment and easy scaling of web applications without complex server setup.

### Why not Virtual Machines
-Using virtual machines requires managing the operating system and installing all necessary software manually.
-App Service simplifies deployment by providing a ready-to-use environment for web applications.
-With virtual machines, the developer is responsible for system maintenance, updates, and security configurations.

### Justification based on cost, scalability, avaliability and workflow:

Cost:
Azure App Service is generally more cost-effective than managing virtual machines. It offers multiple pricing tiers, including Free and Shared plans, which allow developers to test or deploy applications at a lower cost. Built-in load balancing also reduces infrastructure expenses.

Scalability:
Azure App Service allows applications to scale easily. Vertical scaling increases resources such as CPU or memory by changing the service plan. Horizontal scaling increases or decreases the number of running instances of the application.

Availability:
Azure provides global infrastructure with high availability. Applications deployed through App Service can run in Microsoft’s global data centers, ensuring reliable service and uptime.

Workflow:
Azure App Service supports automated deployment from platforms such as GitHub, Azure DevOps, or other Git repositories. Developers can also use GitHub Actions to create workflows that automatically build, test, and deploy applications.

### Assess app changes that would change your decision.

Azure App Service has certain limitations in terms of hardware control and customization. If the application grows significantly in scale, requires specialized configurations, or demands greater control over the system environment, using a Virtual Machine may become more appropriate. For larger applications with increased users or complex system requirements, virtual machines provide greater flexibility and control.