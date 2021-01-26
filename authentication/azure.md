# Azure

When running commands that interact with Azure infrastructure you will have to authenticate with Azure.

## Device Flow Authentication

When using Sumocli in an interactive way the best way to authenticate with Azure is using device code flow. Device code flow outputs a sign-in URL and a one-time code to the console and allows the user to authenticate against an App Registration rather than using an application secret.

The following options are required to use device flow authentication:

* `--clientId` - Client ID of the Enterprise Application.
* `--location` - Azure location to deploy the Infrastructure to.
* `--subscriptionId` - Subscription ID for the subscription that the infrastructure should be deployed to.
* `--tenantId` - Tenant ID of the Azure AD tenant.
* `--useDeviceFlow` - Tells Sumocli to use device flow authentication.

When you configure the App Registration you need to ensure the application has Azure Service Management delegated permissions and Microsoft Graph User.Read delegated permissions.

## Service Principal Authentication

When using Sumocli in a CI/CD pipeline or in a script the best way to authenticate with Azure using a service principal. Currently Sumocli only supports secret based authentication not certificate based.

The following options are require to use service principal authentication:

* `--clientId` - Client ID of the App Registration.
* `--clientSecret` - Client Secret of the App Registration.
* `--location` - Azure location to deploy the Infrastructure to.
* `--subscriptionId` - Subscription ID for the subscription that the infrastructure should be deployed to.
* `--tenantId` - Tenant ID of the Azure AD tenant.

