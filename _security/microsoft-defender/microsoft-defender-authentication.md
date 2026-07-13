---
api_key_in: []
api_specs:
- filename: microsoft-defender-for-endpoint-api-openapi.yml
  format: yaml
  label: Microsoft Defender for Endpoint API
  slug: microsoft-defender-for-endpoint-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/microsoft-defender/refs/heads/main/openapi/microsoft-defender-for-endpoint-api-openapi.yml
- filename: graph-explorer
  format: yaml
  label: Microsoft Graph Security API
  slug: microsoft-graph-security-api
  spec_type: OpenAPI
  url: https://developer.microsoft.com/en-us/graph/graph-explorer
auth_types:
- oauth2
description: ''
kind: authentication
layout: security
method: derived
name: Microsoft Defender Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
- clientCredentials
overview: Microsoft Defender secures its APIs with oauth2 across 1 declared security scheme, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode and clientCredentials flow(s).
provider_name: Microsoft Defender
provider_slug: microsoft-defender
scheme_count: 1
schemes:
- description: OAuth 2.0 authentication using Microsoft Entra ID (Azure AD). Supports both application-level and delegated permissions.
  flows:
  - flow: clientCredentials
    scopes: 1
    tokenUrl: https://login.microsoftonline.com/{tenantId}/oauth2/v2.0/token
  - authorizationUrl: https://login.microsoftonline.com/{tenantId}/oauth2/v2.0/authorize
    flow: authorizationCode
    scopes: 1
    tokenUrl: https://login.microsoftonline.com/{tenantId}/oauth2/v2.0/token
  name: oauth2
  sources:
  - openapi/microsoft-defender-for-endpoint-api-openapi.yml
  type: oauth2
slug: microsoft-defender-authentication
source_filename: microsoft-defender-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/microsoft-defender-for-endpoint-api-openapi.yml\nsummary:\n  types:\n  - oauth2\n  oauth2_flows:\n  - authorizationCode\n  - clientCredentials\nschemes:\n- name: oauth2\n  type: oauth2\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://login.microsoftonline.com/{tenantId}/oauth2/v2.0/token\n    scopes: 1\n  - flow: authorizationCode\n    authorizationUrl: https://login.microsoftonline.com/{tenantId}/oauth2/v2.0/authorize\n    tokenUrl: https://login.microsoftonline.com/{tenantId}/oauth2/v2.0/token\n    scopes: 1\n  description: OAuth 2.0 authentication using Microsoft Entra ID (Azure AD). Supports both application-level\n    and delegated permissions.\n  sources:\n  - openapi/microsoft-defender-for-endpoint-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/microsoft-defender/refs/heads/main/authentication/microsoft-defender-authentication.yml
summary_line: oauth2 · 1 scheme
tags: []
---
