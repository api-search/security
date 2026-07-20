---
api_key_in: []
auth_types:
- oauth2
description: ''
kind: authentication
layout: security
method: searched
name: Code 42 Authentication
name_suffix: Authentication
oauth_flows:
- clientCredentials
overview: Code 42 secures its APIs with oauth2 across 1 declared security scheme, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the clientCredentials flow(s).
provider_name: Code 42
provider_slug: code-42
scheme_count: 1
schemes:
- description: Code42 API clients are OAuth 2.0-compliant. You create an API client in the Code42 console, which issues a client ID, secret, and a tenant-specific base URL (shown only once). Exchange the client ID and secret for a short-lived bearer token, then send that token on every API request.
  flow: clientCredentials
  name: apiClientOAuth
  notes: Tokens expire after 15 minutes (900s). The token endpoint host is region-specific (api.us.code42.com, api.us2.code42.com, api.gov.code42.com, and other regional gateways). Permissions are governed by the role assigned to the API client, not by OAuth scopes; no public scope reference is documented, so no scopes/ artifact is emitted.
  request_header: 'Authorization: Bearer <access_token>'
  token_endpoint: https://api.us.code42.com/v1/oauth
  token_expires_in: 900
  token_request: curl -X POST -u '<ClientID>:<Secret>' -d "" https://api.us.code42.com/v1/oauth
  token_response_example: '{"access_token":"...","token_type":"bearer","expires_in":900}'
  type: oauth2
slug: code-42-authentication
source_filename: code-42-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: searched\nsource: https://developer.code42.com/ + Code42 API clients docs\ndocs: https://developer.code42.com/\nsummary:\n  types:\n  - oauth2\n  oauth2_flows:\n  - clientCredentials\n  token_lifetime_seconds: 900\n  token_type: bearer\nschemes:\n- name: apiClientOAuth\n  type: oauth2\n  flow: clientCredentials\n  description: >-\n    Code42 API clients are OAuth 2.0-compliant. You create an API client in the\n    Code42 console, which issues a client ID, secret, and a tenant-specific base\n    URL (shown only once). Exchange the client ID and secret for a short-lived\n    bearer token, then send that token on every API request.\n  token_endpoint: https://api.us.code42.com/v1/oauth\n  token_request: >-\n    curl -X POST -u '<ClientID>:<Secret>' -d \"\" https://api.us.code42.com/v1/oauth\n  token_response_example: '{\"access_token\":\"...\",\"token_type\":\"bearer\",\"expires_in\":900}'\n  request_header: 'Authorization: Bearer <access_token>'\n\
  \  token_expires_in: 900\n  notes: >-\n    Tokens expire after 15 minutes (900s). The token endpoint host is\n    region-specific (api.us.code42.com, api.us2.code42.com, api.gov.code42.com,\n    and other regional gateways). Permissions are governed by the role assigned\n    to the API client, not by OAuth scopes; no public scope reference is\n    documented, so no scopes/ artifact is emitted.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/code-42/refs/heads/main/authentication/code-42-authentication.yml
summary_line: oauth2 · 1 scheme
tags:
- Company
- Security
- Insider Risk Management
- Data Loss Prevention
- Data Security
- Endpoint Security
- Cybersecurity
- SaaS
---
