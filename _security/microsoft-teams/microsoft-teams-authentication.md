---
api_key_in: []
api_specs:
- filename: microsoft-teams-graph-api.yaml
  format: yaml
  label: Microsoft Graph Teams API
  slug: microsoft-graph-teams-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/microsoft-teams/refs/heads/main/openapi/microsoft-teams-graph-api.yaml
- filename: microsoft-teams-asyncapi.yaml
  format: yaml
  label: Microsoft Teams Bot Framework API
  slug: microsoft-teams-bot-framework-api
  spec_type: AsyncAPI
  url: https://raw.githubusercontent.com/api-evangelist/microsoft-teams/refs/heads/main/asyncapi/microsoft-teams-asyncapi.yaml
auth_types:
- oauth2
description: ''
kind: authentication
layout: security
method: searched
name: Microsoft Teams Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: Microsoft Teams secures its APIs with oauth2 across 1 declared security scheme, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: Microsoft Teams
provider_slug: microsoft-teams
scheme_count: 1
schemes:
- description: OAuth 2.0 authorization using Microsoft Identity Platform
  flows:
  - authorizationUrl: https://login.microsoftonline.com/common/oauth2/v2.0/authorize
    flow: authorizationCode
    scopes: 10
    tokenUrl: https://login.microsoftonline.com/common/oauth2/v2.0/token
  name: oauth2
  sources:
  - openapi/microsoft-teams-graph-api.yaml
  type: oauth2
slug: microsoft-teams-authentication
source_filename: microsoft-teams-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-06-20'\nmethod: searched\nsource: openapi/microsoft-teams-graph-api.yaml\ndocs: https://learn.microsoft.com/en-us/graph/auth/\nidentity_platform: Microsoft Identity Platform (Entra ID)\nconsent_model: delegated and application permissions; admin consent required for high-privilege scopes\nsummary:\n  types:\n  - oauth2\n  oauth2_flows:\n  - authorizationCode\nschemes:\n- name: oauth2\n  type: oauth2\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://login.microsoftonline.com/common/oauth2/v2.0/authorize\n    tokenUrl: https://login.microsoftonline.com/common/oauth2/v2.0/token\n    scopes: 10\n  description: OAuth 2.0 authorization using Microsoft Identity Platform\n  sources:\n  - openapi/microsoft-teams-graph-api.yaml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/microsoft-teams/refs/heads/main/authentication/microsoft-teams-authentication.yml
summary_line: oauth2 · 1 scheme
tags:
- Chat
- Collaboration
- Communication
- Microsoft 365
- Productivity
- Video Conferencing
---
