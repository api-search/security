---
api_key_in: []
auth_types: []
description: ''
kind: authentication
layout: security
method: searched
name: Act On Authentication
name_suffix: Authentication
oauth_flows: []
overview: Act-On declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: Act-On
provider_slug: act-on
scheme_count: 1
schemes:
- flows:
  - description: Exchange username and password for an access_token and refresh_token.
    doc: https://developer.act-on.com/reference/grant-type-password
    grant_type: password
  - description: Exchange a refresh_token for a new access_token and refresh_token.
    doc: https://developer.act-on.com/reference/grant-type-refresh
    grant_type: refresh_token
  - description: Exchange an authorization code for an access_token and refresh_token.
    doc: https://developer.act-on.com/reference/grant-type-code
    grant_type: authorization_code
  name: oauth2
  transmit: Authorization header, Bearer scheme
  type: oauth2
slug: act-on-authentication
source_filename: act-on-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-17'\nmethod: searched\nsource: https://developer.act-on.com/reference/api-overview + live probe of https://restapi.actonsoftware.com/token\napi: Act-On REST API\nsummary: >-\n  Act-On's REST API authenticates with OAuth 2.0. Clients exchange credentials at\n  the token endpoint for a short-lived bearer access_token (sent as\n  Authorization: Bearer <token>) plus a refresh_token used to obtain new access\n  tokens. Three grant types are documented.\ntoken_endpoint: https://restapi.actonsoftware.com/token\ntoken_endpoint_probe:\n  method: POST\n  status: 401\n  body: '{\"error\":\"access_denied\",\"error_description\":\"Unauthorized\"}'\n  note: Unauthenticated POST returns an OAuth2 error object, confirming OAuth2.\nschemes:\n- type: oauth2\n  name: oauth2\n  flows:\n  - grant_type: password\n    doc: https://developer.act-on.com/reference/grant-type-password\n    description: Exchange username and password for an access_token and refresh_token.\n  - grant_type:\
  \ refresh_token\n    doc: https://developer.act-on.com/reference/grant-type-refresh\n    description: Exchange a refresh_token for a new access_token and refresh_token.\n  - grant_type: authorization_code\n    doc: https://developer.act-on.com/reference/grant-type-code\n    description: Exchange an authorization code for an access_token and refresh_token.\n  transmit: Authorization header, Bearer scheme\ndocs: https://developer.act-on.com/reference/api-overview\nnotes:\n- Developer/API access requires an Act-On developer account (see request-a-developer-account).\n- No API-key-only scheme was documented; OAuth 2.0 is the sole documented mechanism.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/act-on/refs/heads/main/authentication/act-on-authentication.yml
summary_line: 1 scheme
tags:
- Company
- Marketing
- Marketing Automation
- Email Marketing
- Email
- Marketing Technology
- Lead Generation
- Campaign Management
- API
---
