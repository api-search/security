---
api_key_in:
- header
auth_types:
- apiKey
- oauth2
description: ''
kind: authentication
layout: security
method: searched
name: Tagove Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: Tagove secures its APIs with apiKey and oauth2 across 2 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: Tagove
provider_slug: tagove
scheme_count: 2
schemes:
- description: 'All REST requests require an API_KEY passed as an HTTP Bearer token in the Authorization header (`Authorization: Bearer {API_KEY}`). Keys are created and revoked under Settings > For Developers > API Key with per-token permissions; keys are shown once and cannot be re-displayed. All requests must be over HTTPS.'
  format: Bearer {API_KEY}
  in: header
  name: ApiKeyBearer
  parameter: Authorization
  sources:
  - https://developer.acquire.io/rest-apis/authorization
  type: apiKey
- description: OAuth is required for publicly-available apps that access other Acquire accounts' data on behalf of users. First-party scripts that access an account's own data use an Access Token instead. Asking users for their Access Token in place of OAuth is against the Acquire terms of service.
  flows:
  - flow: authorizationCode
  name: OAuth2
  sources:
  - https://developer.acquire.io/master/rest-apis/oauth/authorization
  type: oauth2
slug: tagove-authentication
source_filename: tagove-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: searched\nsource: https://developer.acquire.io/rest-apis/authorization\ndocs: https://developer.acquire.io/rest-apis/authorization\nnote: >-\n  Tagove now operates as Acquire.io (acquire.io); this profile documents the\n  Acquire developer platform that succeeded Tagove. No machine-readable OpenAPI\n  is published, so this profile is captured from the developer documentation.\nsummary:\n  types:\n  - apiKey\n  - oauth2\n  api_key_in:\n  - header\n  oauth2_flows:\n  - authorizationCode\nschemes:\n- name: ApiKeyBearer\n  type: apiKey\n  in: header\n  parameter: Authorization\n  format: 'Bearer {API_KEY}'\n  description: >-\n    All REST requests require an API_KEY passed as an HTTP Bearer token in the\n    Authorization header (`Authorization: Bearer {API_KEY}`). Keys are created\n    and revoked under Settings > For Developers > API Key with per-token\n    permissions; keys are shown once and cannot be re-displayed. All requests\n    must be\
  \ over HTTPS.\n  sources:\n  - https://developer.acquire.io/rest-apis/authorization\n- name: OAuth2\n  type: oauth2\n  description: >-\n    OAuth is required for publicly-available apps that access other Acquire\n    accounts' data on behalf of users. First-party scripts that access an\n    account's own data use an Access Token instead. Asking users for their\n    Access Token in place of OAuth is against the Acquire terms of service.\n  flows:\n  - flow: authorizationCode\n  sources:\n  - https://developer.acquire.io/master/rest-apis/oauth/authorization\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/tagove/refs/heads/main/authentication/tagove-authentication.yml
summary_line: apiKey/oauth2 · 2 schemes
tags:
- Company
- Customer Support
- Live Chat
- Conversational
- Co-browsing
- Chatbots
- Webhooks
- Customer Communication
- Help Desk
---
