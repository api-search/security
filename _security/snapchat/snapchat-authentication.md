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
- filename: snapchat-ad-accounts-api-openapi.yml
  format: yaml
  label: Snapchat Ad Accounts API
  slug: snapchat-ad-accounts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/snapchat/refs/heads/main/openapi/snapchat-ad-accounts-api-openapi.yml
- filename: snapchat-ad-squads-api-openapi.yml
  format: yaml
  label: Snapchat Ad Squads API
  slug: snapchat-ad-squads-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/snapchat/refs/heads/main/openapi/snapchat-ad-squads-api-openapi.yml
- filename: snapchat-audience-segments-api-openapi.yml
  format: yaml
  label: Snapchat Audience Segments API
  slug: snapchat-audience-segments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/snapchat/refs/heads/main/openapi/snapchat-audience-segments-api-openapi.yml
- filename: snapchat-campaigns-api-openapi.yml
  format: yaml
  label: Snapchat Campaigns API
  slug: snapchat-campaigns-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/snapchat/refs/heads/main/openapi/snapchat-campaigns-api-openapi.yml
- filename: snapchat-conversion-events-api-openapi.yml
  format: yaml
  label: Snapchat Conversion Events API
  slug: snapchat-conversion-events-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/snapchat/refs/heads/main/openapi/snapchat-conversion-events-api-openapi.yml
- filename: snapchat-creatives-api-openapi.yml
  format: yaml
  label: Snapchat Creatives API
  slug: snapchat-creatives-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/snapchat/refs/heads/main/openapi/snapchat-creatives-api-openapi.yml
- filename: snapchat-funding-sources-api-openapi.yml
  format: yaml
  label: Snapchat Funding Sources API
  slug: snapchat-funding-sources-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/snapchat/refs/heads/main/openapi/snapchat-funding-sources-api-openapi.yml
- filename: snapchat-measurement-api-openapi.yml
  format: yaml
  label: Snapchat Measurement API
  slug: snapchat-measurement-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/snapchat/refs/heads/main/openapi/snapchat-measurement-api-openapi.yml
- filename: snapchat-media-api-openapi.yml
  format: yaml
  label: Snapchat Media API
  slug: snapchat-media-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/snapchat/refs/heads/main/openapi/snapchat-media-api-openapi.yml
- filename: snapchat-oauth-api-openapi.yml
  format: yaml
  label: Snapchat OAuth API
  slug: snapchat-oauth-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/snapchat/refs/heads/main/openapi/snapchat-oauth-api-openapi.yml
- filename: snapchat-organizations-api-openapi.yml
  format: yaml
  label: Snapchat Organizations API
  slug: snapchat-organizations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/snapchat/refs/heads/main/openapi/snapchat-organizations-api-openapi.yml
- filename: snapchat-user-profile-api-openapi.yml
  format: yaml
  label: Snapchat User Profile API
  slug: snapchat-user-profile-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/snapchat/refs/heads/main/openapi/snapchat-user-profile-api-openapi.yml
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
