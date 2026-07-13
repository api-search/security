---
api_key_in:
- query
api_specs:
- filename: snapchat-ads-api-openapi.yml
  format: yaml
  label: Snapchat Ads API
  slug: snapchat-ads-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/snapchat/refs/heads/main/openapi/snapchat-ads-api-openapi.yml
- filename: snapchat-conversions-api-openapi.yml
  format: yaml
  label: Snapchat Conversions API
  slug: snapchat-conversions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/snapchat/refs/heads/main/openapi/snapchat-conversions-api-openapi.yml
- filename: snapchat-login-kit-openapi.yml
  format: yaml
  label: Snapchat Login Kit API
  slug: snapchat-login-kit
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/snapchat/refs/heads/main/openapi/snapchat-login-kit-openapi.yml
auth_types:
- apiKey
- http
- oauth2
description: ''
kind: authentication
layout: security
method: derived
name: Snapchat Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: Snapchat secures its APIs with apiKey, http, and oauth2 across 3 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: Snapchat
provider_slug: snapchat
scheme_count: 3
schemes:
- description: OAuth 2.0 authorization. Access tokens are obtained via the authorization code flow and expire after 3600 seconds. Refresh tokens can be used to obtain new access tokens.
  flows:
  - authorizationUrl: https://accounts.snapchat.com/accounts/oauth2/auth
    flow: authorizationCode
    scopes: 1
    tokenUrl: https://accounts.snapchat.com/login/oauth2/access_token
  name: bearerAuth
  sources:
  - openapi/snapchat-ads-api-openapi.yml
  type: oauth2
- description: Static long-lived access token generated from the Business Details page of Ads Manager.
  in: query
  name: accessToken
  parameter: access_token
  sources:
  - openapi/snapchat-conversions-api-openapi.yml
  type: apiKey
- description: Bearer access token obtained via the OAuth 2.0 authorization code flow. Tokens expire after 3600 seconds.
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/snapchat-login-kit-openapi.yml
  type: http
slug: snapchat-authentication
source_filename: snapchat-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/snapchat-ads-api-openapi.yml, openapi/snapchat-conversions-api-openapi.yml,\n  openapi/snapchat-login-kit-openapi.yml\nsummary:\n  types:\n  - apiKey\n  - http\n  - oauth2\n  api_key_in:\n  - query\n  oauth2_flows:\n  - authorizationCode\nschemes:\n- name: bearerAuth\n  type: oauth2\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://accounts.snapchat.com/accounts/oauth2/auth\n    tokenUrl: https://accounts.snapchat.com/login/oauth2/access_token\n    scopes: 1\n  description: OAuth 2.0 authorization. Access tokens are obtained via the authorization code\n    flow and expire after 3600 seconds. Refresh tokens can be used to obtain new access tokens.\n  sources:\n  - openapi/snapchat-ads-api-openapi.yml\n- name: accessToken\n  type: apiKey\n  in: query\n  parameter: access_token\n  description: Static long-lived access token generated from the Business Details page of Ads\n    Manager.\n  sources:\n \
  \ - openapi/snapchat-conversions-api-openapi.yml\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  description: Bearer access token obtained via the OAuth 2.0 authorization code flow. Tokens\n    expire after 3600 seconds.\n  sources:\n  - openapi/snapchat-login-kit-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/snapchat/refs/heads/main/authentication/snapchat-authentication.yml
summary_line: apiKey/http/oauth2 · 3 schemes
tags:
- Advertising
- AR
- Augmented Reality
- Marketing
- Messaging
- Social Media
---
