![Alt text](readme-assets/logo.jpg?raw=true "CloudExcellence")

# Cloudxcellence

![Slide1](https://github.com/cloudxcellence/cloudxcellence/assets/71469979/dfe5f95d-7980-44b5-8e65-633b73f839d2)
![Slide2](https://github.com/cloudxcellence/cloudxcellence/assets/71469979/6f4ceceb-a265-4334-b4ab-caae4c264d03)

![Slide7](https://github.com/cloudxcellence/cloudxcellence/assets/71469979/183cb4e0-e0cd-42da-845d-f93cb75bc759)




## Marketplace Deployment Steps

### Pre-Deployment
* Gather the below information as mentioned in the table -

| Sl no.        | Parameter Details           | Description  |
| ------------- |:-------------|:-----|
| 1             | Client Id ( or service principle) | A service principle is needed for the CloudXcellence app to fetch the data at the subscription level for multiple resources. |
| 2             | Client Secret      |   The `secret` of the above client id. |
| 3             | Service Principle Object Id      | An Object Id of the above Client Id is also needed for the deployment to succeed. |
| 4             | Send EmailNotifications To          | List of comma separated email ids to send alerts ( under development ) | 
| 5             | Deploy DB          | Default is True, please do not change. | 


### Post-Deployment

Configure the below settings to enable the dashboard. For this you need to go to below sections in your chosen service principle under Azure Active Directory.


* Authentication - Configure the SPA and Grant Types and math the other settings as shown below.
![Alt text](readme-assets/Authentication.png?raw=true "Authentication")

* API permissions - Configure the SPA and Grant Types and math the other settings as shown below.
![Alt text](readme-assets/API_Permissions.jpg?raw=true "API_Permissions")

* Add users - Configure this setting to add the users who would like to access the CloudXcellence dashboard. You can visit this setting from the service principle's overview tab, then `Configure for your organization`, then `Assign users and groups`
![Alt text](readme-assets/Add_Users.jpg?raw=true "Add_Users")
