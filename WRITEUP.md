# Write-up Template

### Analyze, choose, and justify the appropriate resource option for deploying the app.

*For **both** a VM or App Service solution for the CMS app:*
- *Analyze costs, scalability, availability, and workflow*
- *Choose the appropriate solution (VM or App Service) for deploying the app*
- *Justify your choice*


--------VM--------
1.Cost 
  VMs are more expensive because you pay for the full server even when usage is low. You also manage OS updates and maintenance, which adds extra cost.
2.Scalability
  Scaling is mostly manual. You need to resize the VM or create more VMs yourself, which takes time and can cause downtime.
3.Availability
  A single VM has lower availability. If it fails, the app goes down unless you set up multiple VMs, which increases cost.
4.Workflow
  You manage everything — OS, patches, security, software installation, and deployments. It gives control but requires more work.

-------App Service--------
1.Cost
  App Service is cheaper because you only pay for the selected plan, and scaling is built-in. No OS maintenance costs.
2.Scalability
  It scales automatically. You can increase instances or upgrade plans without downtime.
3.Availability
  High availability is built-in. Microsoft manages the infrastructure, so the app stays online even if servers fail.
4.Workflow
  Easy to deploy using GitHub, VS Code, or pipelines. No need to manage OS or servers — only focus on the app.


--------Justify Your Choice--------
I chose App Service because it is easier to manage and requires no server or OS maintenance. It also provides automatic scaling and high availability without extra setup. Overall, it is cheaper, faster to deploy, and more suitable for running a CMS app compared to a VM.


### Assess app changes that would change your decision.

----------Assess app changes that would change your decision----------
I would change my decision and choose a VM if the app required full control over the operating system, custom server configurations, or software that App Service does not support. If the CMS app needed background services, heavy processing, or special networking setups, a VM would be a better choice. In those cases, App Service would not be enough.


*Detail how the app and any other needs would have to change for you to change your decision in the last section.* 