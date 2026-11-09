---
anonymous_access: false
api_key_in: []
auth_types: []
description: ''
kind: authentication
layout: security
mechanism_count: 2
method: searched
name: Microsoft Advertising Authentication
name_suffix: Authentication
oauth_flows: []
overview: Microsoft Advertising declares 2 security scheme(s) across its OpenAPI definitions.
provider_name: Microsoft Advertising
provider_slug: microsoft-advertising
scheme_count: 2
schemes:
- authorizationUrl: https://login.microsoftonline.com/common/oauth2/v2.0/authorize
  flow: authorizationCode
  note: Microsoft identity platform; Google OAuth sign-in is also documented (authentication-oauth-register#register-your-application-with-google-oauth).
  scopes:
  - https://ads.microsoft.com/msads.manage
  - offline_access
  tokenUrl: https://login.microsoftonline.com/common/oauth2/v2.0/token
  type: oauth2
- in: header
  name: DeveloperToken
  note: Every SOAP request carries AuthenticationToken (OAuth access token) and DeveloperToken headers, plus CustomerId/CustomerAccountId where required (get-started).
  type: apiKey
slug: microsoft-advertising-authentication
source_filename: microsoft-advertising-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "name: Microsoft Advertising authentication\ngenerated: '2026-11-04'\nmethod: searched\nsource: https://learn.microsoft.com/en-us/advertising/guides/authentication-oauth\ndocs: https://learn.microsoft.com/en-us/advertising/guides/authentication-oauth-get-tokens\nschemes:\n- type: oauth2\n  flow: authorizationCode\n  authorizationUrl: https://login.microsoftonline.com/common/oauth2/v2.0/authorize\n  tokenUrl: https://login.microsoftonline.com/common/oauth2/v2.0/token\n  scopes:\n  - https://ads.microsoft.com/msads.manage\n  - offline_access\n  note: Microsoft identity platform; Google OAuth sign-in is also documented (authentication-oauth-register#register-your-application-with-google-oauth).\n- type: apiKey\n  in: header\n  name: DeveloperToken\n  note: Every SOAP request carries AuthenticationToken (OAuth access token) and DeveloperToken headers, plus CustomerId/CustomerAccountId where required (get-started).\n"
source_yaml_url: https://artifacts.apis.io/microsoft-advertising/authentication/microsoft-advertising-authentication.yml
summary_line: 2 schemes
tags:
- Advertising
- Analytics
- Bing Ads
- Bulk Operations
- Campaigns
- Microsoft
- Reporting
- SOAP
- Search Advertising
---
