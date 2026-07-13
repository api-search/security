---
api_key_in: []
api_specs:
- filename: openapi.yaml
  format: yaml
  label: Microsoft Graph API
  slug: microsoft-graph-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/microsoftgraph/microsoft-graph-openapi/master/openapi/v1.0/openapi.yaml
- filename: mail.yaml
  format: yaml
  label: Outlook Mail API
  slug: outlook-mail-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/microsoftgraph/microsoft-graph-openapi/master/openapi/v1.0/mail.yaml
- filename: calendar.yaml
  format: yaml
  label: Outlook Calendar API
  slug: outlook-calendar-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/microsoftgraph/microsoft-graph-openapi/master/openapi/v1.0/calendar.yaml
- filename: files.yaml
  format: yaml
  label: OneDrive API
  slug: onedrive-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/microsoftgraph/microsoft-graph-openapi/master/openapi/v1.0/files.yaml
- filename: sites.yaml
  format: yaml
  label: SharePoint API
  slug: sharepoint-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/microsoftgraph/microsoft-graph-openapi/master/openapi/v1.0/sites.yaml
- filename: teams.yaml
  format: yaml
  label: Microsoft Teams API
  slug: microsoft-teams-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/microsoftgraph/microsoft-graph-openapi/master/openapi/v1.0/teams.yaml
- filename: users.yaml
  format: yaml
  label: Office 365 Users API
  slug: office-365-users-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/microsoftgraph/microsoft-graph-openapi/master/openapi/v1.0/users.yaml
- filename: planner.yaml
  format: yaml
  label: Planner API
  slug: planner-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/microsoftgraph/microsoft-graph-openapi/master/openapi/v1.0/planner.yaml
- filename: microsoft-graph-api-openapi.yml
  format: yaml
  label: Office 365 Groups API
  slug: office-365-groups-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/microsoft-office-365/refs/heads/main/openapi/microsoft-graph-api-openapi.yml
auth_types:
- http
- oauth2
description: ''
kind: authentication
layout: security
method: derived
name: Microsoft Office 365 Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
- clientCredentials
overview: Microsoft Office 365 secures its APIs with http and oauth2 across 2 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode and clientCredentials flow(s).
provider_name: Microsoft Office 365
provider_slug: microsoft-office-365
scheme_count: 2
schemes:
- description: Microsoft identity platform OAuth 2.0 authorization. Supports delegated (user) and application-only permissions. Microsoft Graph uses scopes to control access to resources.
  flows:
  - authorizationUrl: https://login.microsoftonline.com/common/oauth2/v2.0/authorize
    flow: authorizationCode
    scopes: 17
    tokenUrl: https://login.microsoftonline.com/common/oauth2/v2.0/token
  - flow: clientCredentials
    scopes: 1
    tokenUrl: https://login.microsoftonline.com/{tenant}/oauth2/v2.0/token
  name: oauth2
  sources:
  - openapi/microsoft-graph-api-openapi.yml
  type: oauth2
- bearerFormat: JWT
  description: Bearer token obtained from the Microsoft identity platform. Use an access token in the Authorization header of each request.
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/microsoft-graph-api-openapi.yml
  type: http
slug: microsoft-office-365-authentication
source_filename: microsoft-office-365-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/microsoft-graph-api-openapi.yml\nsummary:\n  types:\n  - http\n  - oauth2\n  oauth2_flows:\n  - authorizationCode\n  - clientCredentials\nschemes:\n- name: oauth2\n  type: oauth2\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://login.microsoftonline.com/common/oauth2/v2.0/authorize\n    tokenUrl: https://login.microsoftonline.com/common/oauth2/v2.0/token\n    scopes: 17\n  - flow: clientCredentials\n    tokenUrl: https://login.microsoftonline.com/{tenant}/oauth2/v2.0/token\n    scopes: 1\n  description: Microsoft identity platform OAuth 2.0 authorization. Supports delegated (user)\n    and application-only permissions. Microsoft Graph uses scopes to control access to resources.\n  sources:\n  - openapi/microsoft-graph-api-openapi.yml\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  description: Bearer token obtained from the Microsoft identity platform. Use an access token\n\
  \    in the Authorization header of each request.\n  sources:\n  - openapi/microsoft-graph-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/microsoft-office-365/refs/heads/main/authentication/microsoft-office-365-authentication.yml
summary_line: http/oauth2 · 2 schemes
tags:
- Cloud
- Collaboration
- Enterprise
- Microsoft
- Productivity
---
