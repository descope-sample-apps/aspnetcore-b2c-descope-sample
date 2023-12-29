<img width="1400" alt="Screenshot 2023-12-29 at 9 48 13 AM" src="https://github.com/descope-sample-apps/aspnetcore-b2c-descope-sample/assets/32936811/309fd9d3-7d14-4c3e-a02b-81f87901e7b4">

---

# Azure AD B2C + Descope ASP.NET Core Sample App

This open-source sample app, built with ASP.NET Core, demonstrates integration with Azure AD B2C and Descope for user authentication. The application showcases using Azure AD B2C for user authentication in an ASP.NET Core application, leveraging the Microsoft Authentication Library (MSAL) for .NET.

Before running the app, ensure Azure AD B2C and Descope are configured as per the provided instructions [here](https://docs.descope.com/knowledgebase/sso/azureoidc/).

## Table of Contents 📝

1. [Features](#features)
2. [Installation](#installation)
3. [Running the Application](#running-the-application)
4. [Configuring Azure AD B2C and Descope](#configuring-azure-ad-b2c-and-descope)
5. [Issue Reporting](#issue-reporting)
6. [License](#license)

## Features ✨

- **Azure AD B2C Integration**: Seamless integration with Azure AD B2C for user authentication.
- **Descope Authentication**: Leverage Descope as a federated identity provider.
- **ASP.NET Core Identity**: Utilize ASP.NET Core Identity for managing user authentication and authorization.

## Installation 💿

Clone the repository:

```bash
git clone https://github.com/descope-sample-apps/aspnetcore-b2c-descope-sample.git
```

Navigate to the cloned repository directory.

Install dependencies:

```bash
dotnet restore
```

## Configuring Authentication Settings

Open `appsettings.json` file and replace the placeholder values with your actual Azure AD B2C settings:

- **ClientId**: Your Azure AD B2C application Client ID.
- **ClientSecret**: Your Azure AD B2C application Client Secret. You can generate one by following this [guide](https://learn.microsoft.com/en-us/azure/active-directory-b2c/tutorial-register-applications#create-a-client-secret).
- **Domain**: Your Azure AD B2C domain.
- **SignUpSignInPolicyId**: Your Azure AD B2C sign-up/sign-in policy ID.

> **Note:** Since this is an ASP.NET Core application, the app is considered a confidential client and is therefore capable of storing a client secret securely.

## Running the Application 🚀

To start the application:

```bash
dotnet run
```

Navigate to `https://localhost:5109/` in your browser.

## Configuring Azure AD B2C and Descope

Ensure you have correctly configured Azure AD B2C and Descope. Follow the detailed guide [here](https://docs.descope.com/knowledgebase/sso/azureoidc/) for instructions on setting up Azure AD B2C Tenant, registering the application, and configuring Descope as an Identity Provider.

## Issue Reporting ⚠️

For any issues or suggestions, please [open an issue](https://github.com/descope-sample-apps/aspnetcore-b2c-descope-sample/issues) on GitHub.

## License 📜

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.
