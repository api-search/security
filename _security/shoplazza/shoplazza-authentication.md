---
api_key_in:
- header
api_specs:
- filename: shoplazza-admin-openapi-original.json
  format: json
  label: Shoplazza Admin API
  slug: shoplazza-admin-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/shoplazza/refs/heads/main/openapi/shoplazza-admin-openapi-original.json
auth_types:
- oauth2
- apiKey
description: ''
kind: authentication
layout: security
method: searched
name: Shoplazza Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: Shoplazza secures its APIs with oauth2 and apiKey across 2 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: Shoplazza
provider_slug: shoplazza
scheme_count: 2
schemes:
- description: Public apps request access scopes from the merchant during installation and exchange an authorization code for an access token + refresh token. Token is then presented as the access-token header on Admin API calls.
  flow: authorizationCode
  name: OAuth2 (authorization code)
  scopes_ref: scopes/shoplazza-scopes.yml
  source: docs
  type: oauth2
- description: The OAuth-issued access token is presented on every Admin API request via the access-token HTTP header (declared as the operation-level security scheme in the OpenAPI spec).
  in: header
  name: apikey-header-access-token
  parameter_name: access-token
  sources:
  - openapi/shoplazza-admin-openapi-original.json
  type: apiKey
slug: shoplazza-authentication
source_filename: shoplazza-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: searched\nsource: https://www.shoplazza.dev/docs/app/building-blocks/authentication/\ndocs: https://www.shoplazza.dev/docs/app/building-blocks/authentication/\nsummary:\n  types: [oauth2, apiKey]\n  api_key_in: [header]\n  api_key_name: access-token\n  oauth2_flows: [authorizationCode]\n  notes: >-\n    Shoplazza uses OAuth 2.0 (authorization code grant) to authorize third-party\n    public apps. The app receives an access token (with refresh token) that is\n    sent on every Admin API request in the access-token request header. OAuth\n    callbacks and webhooks are additionally verified with an HMAC signature.\n    App Bridge embedded apps use short-lived session tokens.\nschemes:\n- name: OAuth2 (authorization code)\n  type: oauth2\n  flow: authorizationCode\n  description: >-\n    Public apps request access scopes from the merchant during installation and\n    exchange an authorization code for an access token + refresh token. Token is\n\
  \    then presented as the access-token header on Admin API calls.\n  scopes_ref: scopes/shoplazza-scopes.yml\n  source: docs\n- name: apikey-header-access-token\n  type: apiKey\n  in: header\n  parameter_name: access-token\n  description: >-\n    The OAuth-issued access token is presented on every Admin API request via\n    the access-token HTTP header (declared as the operation-level security\n    scheme in the OpenAPI spec).\n  sources: [openapi/shoplazza-admin-openapi-original.json]\nsignature_verification:\n  method: HMAC\n  applies_to: [oauth-callbacks, webhooks]\n  docs: https://www.shoplazza.dev/docs/app/building-blocks/authentication/\nembedded_session_tokens:\n  used_by: App Bridge\n  docs: https://www.shoplazza.dev/docs/app/developer-tools/app-bridge/\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/shoplazza/refs/heads/main/authentication/shoplazza-authentication.yml
summary_line: oauth2/apiKey · 2 schemes
tags:
- Company
- Enterprise
- E-Commerce
- Online Store
- Retail
- Payments
- Webhooks
- REST API
- Apps
- Developer Platform
---
