---
title: Configure an OAuth 2.0 provider for Power Pages
description: Learn how to configure OAuth 2.0 identity providers such as Microsoft, LinkedIn, Facebook, Google, and Twitter in Power Pages.
author: sandhangitmsft

ms.topic: conceptual
ms.custom: 
ms.date: 3/3/2023
ms.author: sandhan
ms.reviewer: kkendrick
contributors:
    - nickdoelman
    - sandhangitmsft
    - dileepsinghmicrosoft
---

# Configure an OAuth 2.0 provider for Power Pages

To use OAuth 2.0&ndash;based external identity providers, you register an application with a third-party service to obtain a *client ID* and *client secret* pair. Often this application requires that you specify a redirect URL to allow the identity provider to send users back to the website (the *relying party*). The client ID and client secret are configured as site settings to establish a secure connection from the relying party to the identity provider. The settings are based on the properties of the [MicrosoftAccountAuthenticationOptions](https://msdn.microsoft.com//library/microsoft.owin.security.microsoftaccount.microsoftaccountauthenticationoptions.aspx), [TwitterAuthenticationOptions](/previous-versions/aspnet/dn450335(v=vs.113)), [FacebookAuthenticationOptions](/previous-versions/aspnet/dn253793(v=vs.113)), and [GoogleOAuth2AuthenticationOptions](/previous-versions/aspnet/dn800251(v=vs.113)) classes.  

To learn about individual OAuth 2.0 providers, select the name of the provider that you want to configure:

- [Microsoft](oauth2-microsoft.md)
- [LinkedIn](oauth2-linkedin.md)
- [Facebook](oauth2-facebook.md)
- [Google](/power-apps/maker/portals/configure/configure-oauth2-google)
- [Twitter](oauth2-twitter.md)

> [!NOTE]
> - Custom OAuth providers aren't supported. For custom OAuth providers, use [OpenID Connect](openid-provider.md) instead.
> Changes to the authentication settings [might take a few minutes](/power-apps/maker/portals/admin/clear-server-side-cache#caching-changes-for-portals-with-version-926x-or-later) to be reflected on the website. Restart the site by using [portal actions](../../admin/admin-overview.md) if you want the changes to be reflected immediately.

For general settings applicable to all OAuth 2.0 providers, go to [Configure additional settings for OAuth 2.0 providers](oauth2-settings.md).

