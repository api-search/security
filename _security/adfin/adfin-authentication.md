---
api_key_in: []
auth_types:
- oauth2
description: ''
kind: authentication
layout: security
method: searched
name: Adfin Authentication
name_suffix: Authentication
oauth_flows:
- clientCredentials
- authorizationCode
overview: Adfin secures its APIs with oauth2 across 3 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the clientCredentials and authorizationCode flow(s).
provider_name: Adfin
provider_slug: adfin
scheme_count: 3
schemes:
- client_auth: basic
  flow: clientCredentials
  name: oauth2_client_credentials
  sources:
  - docs
  tokenUrl: https://api.adfin.com/api/oauth2/token
  tokenUrl_staging: https://api.staging.adfin.com/api/oauth2/token
  type: oauth2
  use: platform-to-platform integrations
- flow: authorizationCode
  name: oauth2_authorization_code
  sources:
  - docs
  type: oauth2
  use: biller authorization (a platform acting on behalf of a biller)
- issuer: https://auth.adfin.com/
  name: auth0_openid_connect
  openIdConnectUrl: https://auth.adfin.com/.well-known/openid-configuration
  sources:
  - well-known/adfin-auth-openid-configuration.json
  type: openIdConnect
  use: console / end-user identity (Auth0)
slug: adfin-authentication
source_filename: adfin-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-17'\nmethod: searched\nsource: https://developer.adfin.com/products/direct-integration/guides/get-started/authentication.md\ndocs: https://developer.adfin.com/products/direct-integration/guides/get-started/authentication.md\nsummary:\n  types: [oauth2]\n  oauth2_flows: [clientCredentials, authorizationCode]\n  api_key_in: []\n  notes: >-\n    The Adfin API uses OAuth 2.0. Platform-to-platform integrations use the\n    client-credentials flow; biller authorization uses the authorization-code\n    flow. App credentials (client_id + client_secret) are issued by an Adfin\n    Integration Manager and presented as HTTP Basic auth against the API's own\n    token endpoint (Basic base64(client_id:client_secret)). This is distinct\n    from the Auth0-backed end-user identity at auth.adfin.com used by the\n    console.\nschemes:\n  - name: oauth2_client_credentials\n    type: oauth2\n    flow: clientCredentials\n    tokenUrl: https://api.adfin.com/api/oauth2/token\n\
  \    tokenUrl_staging: https://api.staging.adfin.com/api/oauth2/token\n    client_auth: basic\n    use: platform-to-platform integrations\n    sources: [docs]\n  - name: oauth2_authorization_code\n    type: oauth2\n    flow: authorizationCode\n    use: biller authorization (a platform acting on behalf of a biller)\n    sources: [docs]\n  - name: auth0_openid_connect\n    type: openIdConnect\n    openIdConnectUrl: https://auth.adfin.com/.well-known/openid-configuration\n    issuer: https://auth.adfin.com/\n    use: console / end-user identity (Auth0)\n    sources: [well-known/adfin-auth-openid-configuration.json]\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/adfin/refs/heads/main/authentication/adfin-authentication.yml
summary_line: oauth2 · 3 schemes
tags:
- Company
- Fintech
- Payments
- Invoicing
- Credit Control
- Direct Debit
- Billing
- Accounts Receivable
- United Kingdom
---
