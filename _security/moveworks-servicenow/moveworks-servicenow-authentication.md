---
api_key_in:
- header
api_specs:
- filename: moveworks-servicenow-data-api-openapi.yml
  format: yaml
  label: Moveworks Data API
  slug: moveworks-data-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/moveworks-servicenow/refs/heads/main/openapi/moveworks-servicenow-data-api-openapi.yml
auth_types:
- http
- oauth2
description: ''
kind: authentication
layout: security
method: searched
name: Moveworks Servicenow Authentication
name_suffix: Authentication
oauth_flows:
- clientCredentials
overview: Moveworks (ServiceNow) secures its APIs with http and oauth2 across 2 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the clientCredentials flow(s).
provider_name: Moveworks (ServiceNow)
provider_slug: moveworks-servicenow
scheme_count: 2
schemes:
- description: 'Bearer token authentication. Supply a long-lived API key, or a short-lived OAuth 2.0 client-credentials access token, in the Authorization header as `Authorization: Bearer <token>`.'
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/moveworks-servicenow-data-api-openapi.yml
  type: http
- description: OAuth 2.0 client-credentials grant (recommended). A Client ID + Client Secret created in the Moveworks dashboard are exchanged at the OAuth token endpoint for a 60-second access token, then presented as a Bearer token.
  flow: clientCredentials
  name: oauth2ClientCredentials
  sources:
  - https://docs.moveworks.com/api-reference/api-credentials
  token_lifetime_seconds: 60
  type: oauth2
slug: moveworks-servicenow-authentication
source_filename: moveworks-servicenow-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: searched\nsource: openapi/moveworks-servicenow-data-api-openapi.yml\ndocs: https://docs.moveworks.com/api-reference/api-credentials\nsummary:\n  types:\n  - http\n  - oauth2\n  api_key_in:\n  - header\n  oauth2_flows:\n  - clientCredentials\nnotes: >-\n  Moveworks REST APIs use Bearer token authentication — the token is sent as\n  `Authorization: Bearer <token>`. Credentials are created in the Moveworks\n  dashboard under HTTP Connectors > Credentials. Two credential types are offered:\n  OAuth 2.0 with Client Credentials (recommended; access tokens generated via the\n  OAuth token endpoint) and long-lived API Keys (validated via the Test Auth\n  endpoint). Client IDs, Client Secrets and API Keys never expire; OAuth access\n  tokens expire after 60 seconds. Credentials are shown in plaintext once at\n  creation and stored only as a hash. Moveworks recommends generating API keys\n  against a dedicated service account rather than an individual\
  \ user account.\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  description: >-\n    Bearer token authentication. Supply a long-lived API key, or a short-lived\n    OAuth 2.0 client-credentials access token, in the Authorization header as\n    `Authorization: Bearer <token>`.\n  sources:\n  - openapi/moveworks-servicenow-data-api-openapi.yml\n- name: oauth2ClientCredentials\n  type: oauth2\n  flow: clientCredentials\n  description: >-\n    OAuth 2.0 client-credentials grant (recommended). A Client ID + Client Secret\n    created in the Moveworks dashboard are exchanged at the OAuth token endpoint\n    for a 60-second access token, then presented as a Bearer token.\n  token_lifetime_seconds: 60\n  sources:\n  - https://docs.moveworks.com/api-reference/api-credentials\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/moveworks-servicenow/refs/heads/main/authentication/moveworks-servicenow-authentication.yml
summary_line: http/oauth2 · 2 schemes
tags:
- Company
- Ai Infrastructure
- AI Assistant
- Agentic AI
- Enterprise Automation
- ITSM
- Conversational AI
- Developer Platform
---
