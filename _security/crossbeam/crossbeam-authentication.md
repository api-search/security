---
api_key_in: []
auth_types:
- oauth2
description: ''
kind: authentication
layout: security
method: searched
name: Crossbeam Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: Crossbeam secures its APIs with oauth2 across 1 declared security scheme, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: Crossbeam
provider_slug: crossbeam
scheme_count: 1
schemes:
- access_token_lifetime: 24h
  audience: https://api.getcrossbeam.com
  authorizationUrl: https://auth.crossbeam.com/authorize?audience=https://api.getcrossbeam.com
  flow: authorizationCode
  name: OAuth2
  refresh: Request the offline_access scope to receive a refresh token; exchange it at the token URL with grant_type=refresh_token for long-running integrations.
  sources:
  - docs
  tokenUrl: https://auth.crossbeam.com/oauth/token
  type: oauth2
slug: crossbeam-authentication
source_filename: crossbeam-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: searched\nsource: https://developers.crossbeam.com/\ndocs:\n  - https://developers.crossbeam.com/\n  - https://help.crossbeam.com/en/articles/4677142-rest-api\n  - https://gitlab.com/crossbeam-public/crossbeam-simple-oauth2\nsummary:\n  types: [oauth2]\n  oauth2_flows: [authorizationCode]\n  api_key_in: []\n  note: >-\n    Public Crossbeam Partner API uses standard OAuth 2.0 (three-legged, authorization-code).\n    Credentials are created as a Custom Integration app in the Crossbeam UI\n    (https://app.crossbeam.com/integrations), which issues a Client ID and Client Secret.\n    Positioned for Enterprise customers.\nschemes:\n  - name: OAuth2\n    type: oauth2\n    flow: authorizationCode\n    authorizationUrl: https://auth.crossbeam.com/authorize?audience=https://api.getcrossbeam.com\n    tokenUrl: https://auth.crossbeam.com/oauth/token\n    audience: https://api.getcrossbeam.com\n    access_token_lifetime: 24h\n    refresh: >-\n      Request\
  \ the offline_access scope to receive a refresh token; exchange it at the token\n      URL with grant_type=refresh_token for long-running integrations.\n    sources: [docs]\nrequired_headers:\n  - name: Authorization\n    value: 'Bearer <access_token>'\n    required: true\n  - name: Xbeam-Organization\n    value: '<organization-uuid>'\n    required: true\n    note: >-\n      Selects which organization's data to return (a user may belong to multiple orgs).\n      Obtain the uuid from GET /v0.1/users/me. Omitting this header is the most common\n      cause of 4xx errors.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/crossbeam/refs/heads/main/authentication/crossbeam-authentication.yml
summary_line: oauth2 · 1 scheme
tags:
- Company
- Ecosystem-Led Growth
- Partnerships
- Account Mapping
- Co-Selling
- Data Collaboration
- Sales Intelligence
- CRM
- Webhooks
- MCP
---
