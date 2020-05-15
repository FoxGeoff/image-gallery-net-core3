# Project: Securing ASP.NET Core 3 with OAuth2 and OpenID Connect

* Online Reference: <https://app.pluralsight.com/library/courses/securing-aspnet-core-3-oauth2-openid-connect/table-of-contents>

## Task: Setting up IdentityServer4

* Add: Project Marvin.IDP (template is4empty)
* Add new templates to Visual Studio ```dotnet new -i IdentityServer4.Templates```

## Task: Project Marvin.IDP

* Run in console: ```image-gallery\src>dotnet new is4empty -n Marvin.IDP```
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

## Task: Add Project for IdentityServer4 Interface 

* Run in console: ```image-gallery\src\Marvin.IDP>dotnet new is4ui```
* Uncomment Startup Code

## Task: Configuring Identy Server

## Task: Loggin in with authorization code flow (client code)

## Task: Enabling PKCE protection
