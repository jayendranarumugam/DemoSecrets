# DemoSecrets

This project is helps us to how we can manage the secrets in the configurations `(appsetting.json)`

**For debuging in local**

`Right click Project`->`Manage user secrets`

Then manage all your secrets in `secrets.json`

**Managing secrets in Azure KeyVault**



update the appsettings.json with corresponding values

`"myConnectionString": <your actual connection string>,
  "Vault": <keyvaultname>, 
  "ClientId": <application id>,  
  "ClientSecret": <application id secret> `
  
  
  Find the full article explaination [here in TechNet](https://social.technet.microsoft.com/wiki/contents/articles/51871.net-core-2-managing-secrets-in-web-apps.aspx)
  
  
 **Priority of getting values from config**
  
1. AzureKeyVault
2. secrets.json
3. appsetting.json
