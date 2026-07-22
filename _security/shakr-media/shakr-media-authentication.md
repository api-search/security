---
api_key_in: []
auth_types:
- oauth2
- http
description: ''
kind: authentication
layout: security
method: searched
name: Shakr Media Authentication
name_suffix: Authentication
oauth_flows:
- clientCredentials
overview: Shakr Media secures its APIs with oauth2 and http across 2 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the clientCredentials flow(s).
provider_name: Shakr Media
provider_slug: shakr-media
scheme_count: 2
schemes:
- flow: clientCredentials
  grant_type: client_credentials
  name: OAuth2ClientCredentials
  params:
  - client_id
  - client_secret
  - grant_type
  - scope
  source: docs
  token_host: https://api.shakr.com
  type: oauth2
- format: Bearer <ACCESS_TOKEN>
  header: Authorization
  in: header
  name: bearerAuth
  scheme: bearer
  source: docs
  type: http
slug: shakr-media-authentication
source_filename: shakr-media-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: searched\nsource: https://developers.shakr.com/docs/api/authentication/\ndocs: https://developers.shakr.com/docs/api/authentication/\nsummary:\n  types: [oauth2, http]\n  api_key_in: []\n  oauth2_flows: [clientCredentials]\n  bearer: true\nnotes: >-\n  The Shakr Video API uses the OAuth 2.0 Client Credentials Grant for\n  service-to-service authentication (no end-user account). Callers exchange a\n  client_id + client_secret (grant_type=client_credentials, optional scope) at\n  the token host for an access_token, then send it as an HTTP bearer token on\n  every request. Access tokens can be scope-restricted using the\n  resource[:action][:target] convention (see scopes/).\nschemes:\n  - name: OAuth2ClientCredentials\n    type: oauth2\n    flow: clientCredentials\n    token_host: https://api.shakr.com\n    grant_type: client_credentials\n    params: [client_id, client_secret, grant_type, scope]\n    source: docs\n  - name: bearerAuth\n    type:\
  \ http\n    scheme: bearer\n    in: header\n    header: Authorization\n    format: \"Bearer <ACCESS_TOKEN>\"\n    source: docs\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/shakr-media/refs/heads/main/authentication/shakr-media-authentication.yml
summary_line: oauth2/http · 2 schemes
tags:
- Company
- Video
- Video Creation
- Video Editing
- Video API
- Media
- SDK
- Automation
- Advertising
- White Label
---
