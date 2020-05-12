# Project: Securing ASP.NET Core 3 with OAuth2 and OpenID Connect

* Online Reference: <https://app.pluralsight.com/library/courses/securing-aspnet-core-3-oauth2-openid-connect/table-of-contents>

## Task: Setting up IdentityServer4

* Add: Project Marvin.IDP (template is4empty)
* Add new templates to Visual Studio ```dotnet new -i IdentityServer4.Templates```

## Task: Project Marvin.IDP

* Change from SelfHost to IIS Express - Debug/Profile-IISExpress (launchSetting.json)
* Run in Console window - Debug/Launch=Project (Edit Project File Wizard)
``` lauchSettings.json
"profiles": {
    "IIS Express": {
      "commandName": "Project",
      "environmentVariables": {
        "ASPNETCORE_ENVIRONMENT": "Development"
      },
      "sqlDebugging": false,
      "applicationUrl": "https://localhost:4431"
    }
  }
```