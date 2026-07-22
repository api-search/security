---
api_key_in:
- header
auth_types:
- apiKey
- oauth2
- openIdConnect
description: ''
kind: authentication
layout: security
method: searched
name: Vindicia Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: Vindicia secures its APIs with apiKey, oauth2, and openIdConnect across 3 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: Vindicia
provider_slug: vindicia
scheme_count: 3
schemes:
- in: header
  name: MerchantApiKey
  sources:
  - https://docs.vindicia.com/bundle/b_merchantOnboardingGuide/page/topics/apiKeys_c.html
  type: apiKey
- flow: authorizationCode
  name: ConnectOAuth2
  sources:
  - https://docs.vindicia.com/bundle/b_ConnectProductDescription/page/topics/oAuth2_c.html
  - https://docs.vindicia.com/bundle/b_ConnectProductDescription/page/topics/tokenScopes_c.html
  type: oauth2
- name: ConnectOIDC
  sources:
  - https://docs.vindicia.com/bundle/b_ConnectProductDescription/page/topics/oAuth2andOpenIDConnect_c.html
  - https://docs.vindicia.com/bundle/b_ConnectProductDescription/page/topics/userInfoEndpoint_c.html
  type: openIdConnect
slug: vindicia-authentication
source_filename: vindicia-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: searched\nsource: https://docs.vindicia.com/bundle/b_Subscribe_REST_API_Guide/page/topics/Authentication.html\ndocs:\n- https://docs.vindicia.com/bundle/b_Subscribe_REST_API_Guide/page/topics/Authentication.html\n- https://docs.vindicia.com/bundle/b_restApiGuide/page/topics/c_apiAuthentication.html\n- https://docs.vindicia.com/bundle/b_merchantOnboardingGuide/page/topics/apiKeys_c.html\n- https://docs.vindicia.com/bundle/b_ConnectProductDescription/page/topics/oAuth2andOpenIDConnect_c.html\nsummary:\n  types:\n  - apiKey\n  - oauth2\n  - openIdConnect\n  api_key_in:\n  - header\n  oauth2_flows:\n  - authorizationCode\nnotes: >-\n  Vindicia's Subscribe and Retain REST APIs authenticate with merchant-issued\n  API keys (managed in the Merchant/Partner portal and passed on the request).\n  Vindicia Connect (the identity/IDP product) additionally documents OAuth 2.0 +\n  OpenID Connect with access tokens, refresh tokens, id tokens, token scopes\
  \ and\n  a userInfo endpoint for external/end-user authentication. Legacy CashBox\n  integrations use the SOAP API. Specific header names and token formats were not\n  captured verbatim (the Zoomin docs render client-side); the auth model above is\n  asserted from the published documentation pages listed under docs[].\nschemes:\n- name: MerchantApiKey\n  type: apiKey\n  in: header\n  sources:\n  - https://docs.vindicia.com/bundle/b_merchantOnboardingGuide/page/topics/apiKeys_c.html\n- name: ConnectOAuth2\n  type: oauth2\n  flow: authorizationCode\n  sources:\n  - https://docs.vindicia.com/bundle/b_ConnectProductDescription/page/topics/oAuth2_c.html\n  - https://docs.vindicia.com/bundle/b_ConnectProductDescription/page/topics/tokenScopes_c.html\n- name: ConnectOIDC\n  type: openIdConnect\n  sources:\n  - https://docs.vindicia.com/bundle/b_ConnectProductDescription/page/topics/oAuth2andOpenIDConnect_c.html\n  - https://docs.vindicia.com/bundle/b_ConnectProductDescription/page/topics/userInfoEndpoint_c.html\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/vindicia/refs/heads/main/authentication/vindicia-authentication.yml
summary_line: apiKey/oauth2/openIdConnect · 3 schemes
tags:
- Company
- Fintech
- Subscription Billing
- Recurring Payments
- Payment Recovery
- Subscription Management
- Payments
- Churn
---
