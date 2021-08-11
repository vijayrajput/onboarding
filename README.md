# onboarding

1. In your web browser, open the [SAP BTP Trial cockpit](https://cockpit.hanatrial.ondemand.com)

2. Navigate to the trial global account by clicking Go To Your Trial Account.
![Image](https://developers.sap.com/tutorials/cp-starter-ibpm-employeeonboarding-1-setup/_jcr_content.github-proxy.1626939075.file/FoundationOnboarding_Home.png)

If this is your first time accessing your trial account, you’ll have to configure your account by choosing a region (*select the region closest to you*). Your user profile will be set up for you automatically.

Wait till your account is set up and ready to go. Your global account, your subaccount, your organization, and your space are launched. This may take a couple of minutes.

Choose Continue.
![Image](https://developers.sap.com/tutorials/cp-starter-ibpm-employeeonboarding-1-setup/_jcr_content.github-proxy.1626939075.file/02_Foundation20Onboarding_Processing.png)

3. From your global account page, choose the Boosters from left-hand navigation. Among the available options, click Start of Set up account for Workflow Management.
![Image](https://developers.sap.com/tutorials/cp-starter-ibpm-employeeonboarding-1-setup/_jcr_content.github-proxy.1626939075.file/startrecipe_21.png)

Automated onboarding will be started with pre-configured steps.
![Image](https://developers.sap.com/tutorials/cp-starter-ibpm-employeeonboarding-1-setup/_jcr_content.github-proxy.1626939075.file/startrecipe_51.png)

4. Click SAP Business Application Studio to launch SAP Business Application Studio.
![Image](https://developers.sap.com/tutorials/appstudio-onboarding/_jcr_content.github-proxy.1614933779.file/BTP-Access-AppStudio-.png)
In the application studio, choose Create Dev Space.
![Image](https://developers.sap.com/tutorials/cp-workflow-2-create-module-cf/_jcr_content.github-proxy.1628162127.file/create-dev-space2.png)

5. Create Dev Space -> Enter a name, for example, mydevspace, and make sure to select SAP Fiori kind and the Workflow Management extension. Then choose Create Dev Space again.
![Image](https://developers.sap.com/tutorials/cp-workflow-2-create-module-cf/_jcr_content.github-proxy.1628162127.file/mydevspace.png)
Wait until the dev space is created and you see the RUNNING status
![Image](https://developers.sap.com/tutorials/cp-workflow-2-create-module-cf/_jcr_content.github-proxy.1628162127.file/DevSpaceCreated.png)

6. BAS Welcome Screen -> Click on Clone from GIT and provide following Repository link  
```
https://github.com/vijayrajput/onboarding.git
```
![Image](https://developers.sap.com/tutorials/cp-workflow-2-create-module-cf/_jcr_content.github-proxy.1628162127.file/see-result-projects-folder.png)


7. Right-click the mta.yaml file in your onboarding project folder, and then select Build MTA Project.
![Image](https://developers.sap.com/tutorials/cp-workflow-3-add-usertask-cf/_jcr_content.github-proxy.1620714027.file/build-mta.png)

Check whether the blue message line at the bottom of your screen, asks you to log in to your Cloud Foundry space.
![Image](https://developers.sap.com/tutorials/cp-workflow-3-add-usertask-cf/_jcr_content.github-proxy.1620714027.file/blue-login-message.png)

Open Login Dialog
If so, click it to open the entry field. Enter the right API endpoint depending on your region, for example, https://api.cf.eu10.hana.ondemand.com, your username and password, and select the Cloud Foundry org and space of your trial account.

8. Right-click the .mtar file, and then select Deploy MTA Archive.
![Image](https://developers.sap.com/tutorials/cp-workflow-3-add-usertask-cf/_jcr_content.github-proxy.1620714027.file/deploy-mtar2.png)

9. From the navigation area, choose Instances and Subscriptions, and search for Workflow Management.

Open your SAP Fiori launchpad, by choosing Go to Application in the Workflow Management row.
![Image](https://developers.sap.com/tutorials/cp-workflow-3-add-usertask-cf/_jcr_content.github-proxy.1620714027.file/go-to-application.png)

10. In the SAP Fiori launchpad, open the Monitor Workflows (Workflow Definitions) application and select the onboard workflow definition.

Choose Start New Instance.
![Image](https://developers.sap.com/tutorials/cp-workflow-3-add-usertask-cf/_jcr_content.github-proxy.1620714027.file/start-new-instance.png)

11. Replace the payload by adding the following code as context, then choose Start New Instance and Close.

```
{
  "managerId": "john.edrich@sapdemo.com",
  "buddyId": "kevin.hart@saptest.com",
  "userId": "cgrant1",
  "empData": {
    "firstName": "Carla",
    "lastName": "Grant",
    "city": "San Mateo",
    "country": "United States",
    "hireDate": "2020-07-11",
    "jobTitle": "General Manager, Industries"
  }
}
```
![Image](https://developers.sap.com/tutorials/cp-workflow-3-add-usertask-cf/_jcr_content.github-proxy.1620714027.file/payload-start-new-instance.png)

12. Go back to the home page and open the My Inbox application.

You should see the Approval task with a form, showing the equipment name and an Approve button.

![Image](https://developers.sap.com/tutorials/cp-workflow-3-add-usertask-cf/_jcr_content.github-proxy.1620714027.file/approve-equipment.png)

