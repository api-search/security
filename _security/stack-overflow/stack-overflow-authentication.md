---
api_key_in: []
api_specs:
- filename: stack-overflow-openapi.yml
  format: yaml
  label: Stack Overflow API
  slug: stack-overflow-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/stack-overflow/refs/heads/main/openapi/stack-overflow-openapi.yml
- filename: stack-overflow-for-teams-openapi.yml
  format: yaml
  label: Stack Overflow for Teams API v3
  slug: stack-overflow-for-teams-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/stack-overflow/refs/heads/main/openapi/stack-overflow-for-teams-openapi.yml
auth_types:
- http
- oauth2
description: ''
kind: authentication
layout: security
method: derived
name: Stack Overflow Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: Stack Overflow secures its APIs with http and oauth2 across 2 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: Stack Overflow
provider_slug: stack-overflow
scheme_count: 2
schemes:
- description: Personal Access Token (PAT) authentication. Pass your PAT as a Bearer token in the Authorization header. Generate tokens from your Stack Overflow for Teams account settings.
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/stack-overflow-for-teams-openapi.yml
  type: http
- description: OAuth 2.0 authentication. Register an application at http://stackapps.com/apps/oauth to obtain credentials.
  flows:
  - authorizationUrl: https://stackoverflow.com/oauth
    flow: authorizationCode
    scopes: 3
    tokenUrl: https://stackoverflow.com/oauth/access_token/json
  name: oauth2
  sources:
  - openapi/stack-overflow-openapi.yml
  type: oauth2
slug: stack-overflow-authentication
source_filename: stack-overflow-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/stack-overflow-for-teams-openapi.yml, openapi/stack-overflow-openapi.yml\nsummary:\n  types:\n  - http\n  - oauth2\n  oauth2_flows:\n  - authorizationCode\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  description: Personal Access Token (PAT) authentication. Pass your PAT as a Bearer token in\n    the Authorization header. Generate tokens from your Stack Overflow for Teams account settings.\n  sources:\n  - openapi/stack-overflow-for-teams-openapi.yml\n- name: oauth2\n  type: oauth2\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://stackoverflow.com/oauth\n    tokenUrl: https://stackoverflow.com/oauth/access_token/json\n    scopes: 3\n  description: OAuth 2.0 authentication. Register an application at http://stackapps.com/apps/oauth\n    to obtain credentials.\n  sources:\n  - openapi/stack-overflow-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/stack-overflow/refs/heads/main/authentication/stack-overflow-authentication.yml
summary_line: http/oauth2 · 2 schemes
tags:
- Answers
- Code
- Developer Community
- Developer Tools
- Knowledge Base
- Programming
- Q&A
- Questions
- Stack Overflow
---
