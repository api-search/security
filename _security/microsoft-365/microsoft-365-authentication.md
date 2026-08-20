---
api_key_in: []
api_specs:
- filename: microsoft-365-calendar-api-openapi.yml
  format: yaml
  label: Microsoft 365 Calendar API
  slug: microsoft-365-calendar-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/microsoft-365/refs/heads/main/openapi/microsoft-365-calendar-api-openapi.yml
- filename: microsoft-365-files-api-openapi.yml
  format: yaml
  label: Microsoft 365 Files API
  slug: microsoft-365-files-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/microsoft-365/refs/heads/main/openapi/microsoft-365-files-api-openapi.yml
- filename: microsoft-365-groups-api-openapi.yml
  format: yaml
  label: Microsoft 365 Groups API
  slug: microsoft-365-groups-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/microsoft-365/refs/heads/main/openapi/microsoft-365-groups-api-openapi.yml
- filename: microsoft-365-mail-api-openapi.yml
  format: yaml
  label: Microsoft 365 Mail API
  slug: microsoft-365-mail-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/microsoft-365/refs/heads/main/openapi/microsoft-365-mail-api-openapi.yml
- filename: microsoft-365-me-api-openapi.yml
  format: yaml
  label: Microsoft 365 Me API
  slug: microsoft-365-me-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/microsoft-365/refs/heads/main/openapi/microsoft-365-me-api-openapi.yml
- filename: microsoft-365-teams-api-openapi.yml
  format: yaml
  label: Microsoft 365 Teams API
  slug: microsoft-365-teams-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/microsoft-365/refs/heads/main/openapi/microsoft-365-teams-api-openapi.yml
- filename: microsoft-365-users-api-openapi.yml
  format: yaml
  label: Microsoft 365 Users API
  slug: microsoft-365-users-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/microsoft-365/refs/heads/main/openapi/microsoft-365-users-api-openapi.yml
auth_types:
- oauth2
description: ''
kind: authentication
layout: security
method: derived
name: Microsoft 365 Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
- clientCredentials
overview: Microsoft 365 secures its APIs with oauth2 across 1 declared security scheme, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode and clientCredentials flow(s).
provider_name: Microsoft 365
provider_slug: microsoft-365
scheme_count: 1
schemes:
- description: Microsoft Entra ID OAuth 2.0
  flows:
  - authorizationUrl: https://login.microsoftonline.com/common/oauth2/v2.0/authorize
    flow: authorizationCode
    scopes: 7
    tokenUrl: https://login.microsoftonline.com/common/oauth2/v2.0/token
  - flow: clientCredentials
    scopes: 1
    tokenUrl: https://login.microsoftonline.com/common/oauth2/v2.0/token
  name: oauth2
  sources:
  - openapi/microsoft-365-openapi.yml
  type: oauth2
slug: microsoft-365-authentication
source_filename: microsoft-365-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/microsoft-365-openapi.yml\nsummary:\n  types:\n  - oauth2\n  oauth2_flows:\n  - authorizationCode\n  - clientCredentials\nschemes:\n- name: oauth2\n  type: oauth2\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://login.microsoftonline.com/common/oauth2/v2.0/authorize\n    tokenUrl: https://login.microsoftonline.com/common/oauth2/v2.0/token\n    scopes: 7\n  - flow: clientCredentials\n    tokenUrl: https://login.microsoftonline.com/common/oauth2/v2.0/token\n    scopes: 1\n  description: Microsoft Entra ID OAuth 2.0\n  sources:\n  - openapi/microsoft-365-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/microsoft-365/refs/heads/main/authentication/microsoft-365-authentication.yml
summary_line: oauth2 · 1 scheme
tags:
- Productivity
- Collaboration
- Email
- Calendar
- File
- Identity
- Microsoft
- Microsoft Graph
---
