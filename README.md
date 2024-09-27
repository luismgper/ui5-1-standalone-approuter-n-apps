# ui5-1-standalone-approuter-n-apps

This is an example of two independent empty applications that can be deployed separatedly using a single standalone approuter as single entrypoint.

The authorization to access can be configured in their respective xs-app.json file. Take notice test-app1 is secured with a role.

To access an app, add to thegenerated approuter endpoint in Cloud Foundry the corresponding app ID at the end

For example por test-app1: https://XXXXXXXXXX-test-multiapprouter-approuter.cfapps.us10-001.hana.ondemand.com/testapp1/index.html

Each app MTA should have the approuter destination service. in this case test-multiapprouter-destination-service, as an existing service.

As indicated in https://help.sap.com/docs/btp/sap-business-technology-platform/deploying-content, html5-apps-repo instance is individual to each application deployment to avoid problems.