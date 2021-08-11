# onboarding

https://cockpit.hanatrial.ondemand.com/

Go To Your Trial Account

Boosters -> Set up account for Workflow Management

Click on Sub-Account - trial -> Instances and Subscriptions -> Subscrptions -> SAP Business Application Studio

Create Dev Space -> Enter a name, for example, mydevspace, and make sure to select SAP Fiori kind and the Workflow Management extension. Then choose Create Dev Space again.

Welcome Screen - > Clone from GIT -> https://github.com/vijayrajput/onboarding.git

Right-click the mta.yaml file in your onboarding project folder, and then select Build MTA Project.

Check whether the blue message line at the bottom of your screen, asks you to log in to your Cloud Foundry space.

Open Login Dialog
If so, click it to open the entry field. Enter the right API endpoint depending on your region, for example, https://api.cf.eu10.hana.ondemand.com, your username and password, and select the Cloud Foundry org and space of your trial account.

Right-click the .mtar file, and then select Deploy MTA Archive.

From the navigation area, choose Instances and Subscriptions, and search for Workflow Management.

Open your SAP Fiori launchpad, by choosing Go to Application in the Workflow Management row.

In the SAP Fiori launchpad, open the Monitor Workflows (Workflow Definitions) application and select the onboard workflow definition.

Choose Start New Instance.

Replace the payload by adding the following code as context, then choose Start New Instance and Close.

'
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


Go back to the home page and open the My Inbox application.

You should see the Approval task with a form, showing the equipment name and an Approve button.



