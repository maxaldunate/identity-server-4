# Introduction to IdentityServer for ASP.NET Core

## Microsoft Virtual Academy Identity Server 4 NET Core Course

* [Microsoft Virtual Academy](https://mva.microsoft.com/en-us/training-courses/introduction-to-identityserver-for-aspnet-core-17945)
* [Brock Allen](https://brockallen.com/)

### Content

1. [Overview of Securing Modern Apps and APIs](#1-overview-of-securing-modern-apps-and-apis)
2. [IdentityServer for ASP.NET Core](#2-identityserver-for-aspnet-core)
3. [Set Up IdentityServer and MVC Client](#3-set-up-identityserver-and-mvc-client)
4. [Set Up and ASP.NET Core Web API](#4-set-up-and-aspnet-core-web-api)
5. [Post.Course Survey](#5-post-course-survey)

### 1. Overview of Securing Modern Apps and APIs

1. [IdentityServer.io WebSite](http://identityserver.io/)
1. [IdentityServer 4 Documentation](https://identityserver4.readthedocs.io/en/release/)
1. [OpenID Connect](http://openid.net/connect/)
1. [OAuth 2](https://oauth.net/2/)
1. [JWT - JSON Web Tokens](https://jwt.io/)

* Competitors
1. [PingFederate Server](https://documentation.pingidentity.com/pingfederate/pf90/index.shtml#gettingStartedGuide/concept/gettingStarted.html)
1. [Azure Active Directory](https://docs.microsoft.com/en-us/azure/active-directory/active-directory-whatis) - [Pricing](https://azure.microsoft.com/en-us/pricing/details/active-directory/)
1. [Okta](https://www.okta.com/)
1. [Auth0](https://auth0.com/)

### 2. IdentityServer for ASP.NET Core

* IdSvr Solucion
  - IdSvrHost. STS 
  - MvcApp. Web App needs login
  - WebApi. API's needs scurity
* On server app.UseIdentityServer();
* [Admin UI](http://www.identityserver.com/documentation/admin-ui/)

> ASP.NET Identity
> MS built in ASP.NET Core is it is a framework for managing the ddbb that contains users authentication information
> Includes: password, MFA, email confirmation, verify mobile phone

* Resources
  - [IdentityServer4 Github](https://github.com/IdentityServer/IdentityServer4/)
  - [IdentityServer4.Samples](https://github.com/IdentityServer/IdentityServer4.Samples)
  - [ASP.NET Core Overview](https://www.asp.net/core/overview/)


* On client 
  - Microsoft.AspNetCore.Authentication.Cookies
  - Microsoft.AspNetCore.Authentication.OpenIdConnect

* In login mvcApp
  - return Challenge();
  - that call HttpContext.Authentication.ChallengeAsync()
  - returning a new ChallengeResult()

### 3. Set Up IdentityServer and MVC Client
### 4. Set Up and ASP.NET Core Web API
### 5. Post Course Survey


The End