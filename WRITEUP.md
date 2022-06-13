# Write-up Template

### Analyze, choose, and justify the appropriate resource option for deploying the app.

*For **both** a VM or App Service solution for the CMS app:*
- *Analyze costs, scalability, availability, and workflow*
- *Choose the appropriate solution (VM or App Service) for deploying the app*
- *Justify your choice*

| Criteria      | VM | App Service |
| ----------- | ----------- | ----------- |
| Cost      | Higher Costs at the beginning - reserved instances possible - pay per instance | Lower Costs at the beginning  - usage driven costs     |
| Scalability   | - Access possible to server configuration - Higher resposibility for configuration | - Not possible to get access to server configurations to analyze performance issues - no multideployments - vertical scaling |
| Availability | Much better availability | Not for high availability |
| Workflow | More maintenance necessary, more efford to integrate in development workflow | Less maintenance, easy integrated in ci/cd of git |

My solution -> App Service (because of lower costs at the beginning for this straightforward application)

### Assess app changes that would change your decision.

*Detail how the app and any other needs would have to change for you to change your decision in the last section.* 
- Other applications run on the VM aswell -> VM
- Not straightforward application -> VM
- Hardware restrictions -> VM
