---
api_key_in: []
api_specs:
- filename: microsoft-teams-asyncapi.yaml
  format: yaml
  label: Microsoft Teams Bot Framework API
  slug: microsoft-teams-bot-framework-api
  spec_type: AsyncAPI
  url: https://raw.githubusercontent.com/api-evangelist/microsoft-teams/refs/heads/main/asyncapi/microsoft-teams-asyncapi.yaml
- filename: microsoft-teams-apps-api-openapi.yml
  format: yaml
  label: Microsoft Teams Apps API
  slug: microsoft-teams-apps-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/microsoft-teams/refs/heads/main/openapi/microsoft-teams-apps-api-openapi.yml
- filename: microsoft-teams-calls-api-openapi.yml
  format: yaml
  label: Microsoft Teams Calls API
  slug: microsoft-teams-calls-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/microsoft-teams/refs/heads/main/openapi/microsoft-teams-calls-api-openapi.yml
- filename: microsoft-teams-channels-api-openapi.yml
  format: yaml
  label: Microsoft Teams Channels API
  slug: microsoft-teams-channels-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/microsoft-teams/refs/heads/main/openapi/microsoft-teams-channels-api-openapi.yml
- filename: microsoft-teams-members-api-openapi.yml
  format: yaml
  label: Microsoft Teams Members API
  slug: microsoft-teams-members-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/microsoft-teams/refs/heads/main/openapi/microsoft-teams-members-api-openapi.yml
- filename: microsoft-teams-messages-api-openapi.yml
  format: yaml
  label: Microsoft Teams Messages API
  slug: microsoft-teams-messages-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/microsoft-teams/refs/heads/main/openapi/microsoft-teams-messages-api-openapi.yml
- filename: microsoft-teams-online-meetings-api-openapi.yml
  format: yaml
  label: Microsoft Teams Online Meetings API
  slug: microsoft-teams-online-meetings-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/microsoft-teams/refs/heads/main/openapi/microsoft-teams-online-meetings-api-openapi.yml
- filename: microsoft-teams-tabs-api-openapi.yml
  format: yaml
  label: Microsoft Teams Tabs API
  slug: microsoft-teams-tabs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/microsoft-teams/refs/heads/main/openapi/microsoft-teams-tabs-api-openapi.yml
- filename: microsoft-teams-teams-api-openapi.yml
  format: yaml
  label: Microsoft Teams Teams API
  slug: microsoft-teams-teams-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/microsoft-teams/refs/heads/main/openapi/microsoft-teams-teams-api-openapi.yml
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
- Communications
- Microsoft-365
- Productivity
- Video Conferencing
---
