---
api_key_in: []
api_specs:
- filename: openapi
  format: yaml
  label: Microsoft Graph API
  slug: microsoft-graph-api
  spec_type: OpenAPI
  url: https://developer.microsoft.com/en-us/graph/docs/concepts/openapi
auth_types:
- oauth2
description: ''
kind: authentication
layout: security
method: derived
name: Microsoft 365 Copilot Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
- clientCredentials
overview: Microsoft 365 Copilot secures its APIs with oauth2 across 1 declared security scheme, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode and clientCredentials flow(s).
provider_name: Microsoft 365 Copilot
provider_slug: microsoft-365-copilot
scheme_count: 1
schemes:
- description: Microsoft Entra ID OAuth 2.0
  flows:
  - authorizationUrl: https://login.microsoftonline.com/common/oauth2/v2.0/authorize
    flow: authorizationCode
    scopes: 6
    tokenUrl: https://login.microsoftonline.com/common/oauth2/v2.0/token
  - flow: clientCredentials
    scopes: 1
    tokenUrl: https://login.microsoftonline.com/common/oauth2/v2.0/token
  name: oauth2
  sources:
  - openapi/microsoft-365-copilot-openapi.yml
  type: oauth2
slug: microsoft-365-copilot-authentication
source_filename: microsoft-365-copilot-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/microsoft-365-copilot-openapi.yml\nsummary:\n  types:\n  - oauth2\n  oauth2_flows:\n  - authorizationCode\n  - clientCredentials\nschemes:\n- name: oauth2\n  type: oauth2\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://login.microsoftonline.com/common/oauth2/v2.0/authorize\n    tokenUrl: https://login.microsoftonline.com/common/oauth2/v2.0/token\n    scopes: 6\n  - flow: clientCredentials\n    tokenUrl: https://login.microsoftonline.com/common/oauth2/v2.0/token\n    scopes: 1\n  description: Microsoft Entra ID OAuth 2.0\n  sources:\n  - openapi/microsoft-365-copilot-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/microsoft-365-copilot/refs/heads/main/authentication/microsoft-365-copilot-authentication.yml
summary_line: oauth2 · 1 scheme
tags:
- Artificial Intelligence
- Copilot
- Enterprise
- LLM
- Microsoft 365
- Natural Language Processing
- Productivity
---
