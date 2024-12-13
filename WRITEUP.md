# Write-up Template

### Analyze, choose, and justify the appropriate resource option for deploying the app.

*For **both** a VM or App Service solution for the CMS app:*
- *Analyze costs, scalability, availability, and workflow*
- *Choose the appropriate solution (VM or App Service) for deploying the app*
- *Justify your choice*

### Assess app changes that would change your decision.

*Detail how the app and any other needs would have to change for you to change your decision in the last section.* 

My answer:

Choosing between VM and WebApp:

In a real world situation, I would recommend developing a two-tier approach for the resource options:
1. Initially implement a WebApp resource.
2. Switch to VM if conditions change after project deployment to Production.

Reasons for initially choosing WebApp:
1. There is no information on who this App is for and how what is the user scope, i.e. will the App be open only for a small community or be available globally?  Therefore I would recommend approaching scalability conservatively.
2. VM seems to be cheaper to setup than WebApp.  WebApp requires a paid subscription, so there is a risk of minimal benefits if the WebApp is not utilized to its fullest.  However, this can be managed with cost monitoring and cutting the subscription if the project is not successful.
3. Even though there is no specified requirement for high Availability, I would say at this point that both options have a high availability feature.  Therefore theoretically they are at a tie for this criteria.
4. The workflow of a VM offers several advantages over WebApp, such as flexibility, performance and hosting.  However the question to ask is "is it needed at this stage of the project?"  Probably not.  Therefore we will choose the approach which will be simpler to deploy.


Factors to consider if changes are needed in my decision:

As mentioned above, a two-tier approach allows the project team an open mind to accept that with changing requirements, the strategy should be changed as well.  Some factors to consider are:
1. Scalability - if the storage limits are exceeded on the WebApp subscription plan, then either upgrade the subscription of switch to VM.
2. Actual Cost to Benefit ratio - if these key figures do not make sense from a financial point of view, then consider switching to VM.  The initial subscription strategy might have been good on paper but may otherwise be proven disadvantageous after Production deployment.

