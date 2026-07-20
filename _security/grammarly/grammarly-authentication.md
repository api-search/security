---
api_key_in: []
auth_types:
- oauth2
description: ''
kind: authentication
layout: security
method: searched
name: Grammarly Authentication
name_suffix: Authentication
oauth_flows:
- clientCredentials
overview: Grammarly secures its APIs with oauth2 across 1 declared security scheme, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the clientCredentials flow(s).
provider_name: Grammarly
provider_slug: grammarly
scheme_count: 1
schemes:
- credential_source: Client ID and Client Secret are issued from the Grammarly Admin panel (Organization > Configurations > OAuth 2.0 credentials). Each credential is assigned one or more OAuth scopes limiting it to specific APIs.
  flow: clientCredentials
  name: OAuth2ClientCredentials
  request_auth:
    format: Bearer <access_token>
    header: Authorization
  sources:
  - developer.grammarly.com/oauth-credentials.html
  token_request:
    method: POST
    parameters:
    - grant_type
    - client_id
    - client_secret
    - scope
  token_url: https://auth.grammarly.com/v4/api/oauth2/token
  type: oauth2
slug: grammarly-authentication
source_filename: grammarly-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: searched\nsource: https://developer.grammarly.com/oauth-credentials.html\ndocs: https://developer.grammarly.com/your-first-api-request.html\nsummary:\n  types: [oauth2]\n  oauth2_flows: [clientCredentials]\n  api_key_in: []\n  token_endpoint: https://auth.grammarly.com/v4/api/oauth2/token\n  transport: Bearer access token in the Authorization header\nschemes:\n- name: OAuth2ClientCredentials\n  type: oauth2\n  flow: clientCredentials\n  token_url: https://auth.grammarly.com/v4/api/oauth2/token\n  token_request:\n    method: POST\n    parameters: [grant_type, client_id, client_secret, scope]\n  credential_source: >-\n    Client ID and Client Secret are issued from the Grammarly Admin panel\n    (Organization > Configurations > OAuth 2.0 credentials). Each credential is\n    assigned one or more OAuth scopes limiting it to specific APIs.\n  request_auth:\n    header: Authorization\n    format: Bearer <access_token>\n  sources: [developer.grammarly.com/oauth-credentials.html]\n\
  notes: >-\n  Grammarly's enterprise developer APIs authenticate with OAuth 2.0 using the\n  client-credentials grant. A machine-to-machine access token is obtained from\n  the token endpoint with the org-issued client_id/client_secret plus the\n  requested scope, then presented as a Bearer token against the API base URL\n  https://api.grammarly.com/ecosystem/api/. See scopes/grammarly-scopes.yml for\n  the scope catalog.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/grammarly/refs/heads/main/authentication/grammarly-authentication.yml
summary_line: oauth2 · 1 scheme
tags:
- Company
- Ai
- Writing Assistance
- Productivity
- Natural Language Processing
- Analytics
- Content
- OAuth
- Enterprise
---
