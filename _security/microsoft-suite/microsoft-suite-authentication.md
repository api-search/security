---
api_key_in: []
api_specs:
- filename: microsoft-suite-calendar-api-openapi.yml
  format: yaml
  label: Microsoft Suite Calendar API
  slug: microsoft-suite-calendar-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/microsoft-suite/refs/heads/main/openapi/microsoft-suite-calendar-api-openapi.yml
- filename: microsoft-suite-files-api-openapi.yml
  format: yaml
  label: Microsoft Suite Files API
  slug: microsoft-suite-files-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/microsoft-suite/refs/heads/main/openapi/microsoft-suite-files-api-openapi.yml
- filename: microsoft-suite-groups-api-openapi.yml
  format: yaml
  label: Microsoft Suite Groups API
  slug: microsoft-suite-groups-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/microsoft-suite/refs/heads/main/openapi/microsoft-suite-groups-api-openapi.yml
- filename: microsoft-suite-mail-api-openapi.yml
  format: yaml
  label: Microsoft Suite Mail API
  slug: microsoft-suite-mail-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/microsoft-suite/refs/heads/main/openapi/microsoft-suite-mail-api-openapi.yml
- filename: microsoft-suite-subscriptions-api-openapi.yml
  format: yaml
  label: Microsoft Suite Subscriptions API
  slug: microsoft-suite-subscriptions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/microsoft-suite/refs/heads/main/openapi/microsoft-suite-subscriptions-api-openapi.yml
- filename: microsoft-suite-teams-api-openapi.yml
  format: yaml
  label: Microsoft Suite Teams API
  slug: microsoft-suite-teams-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/microsoft-suite/refs/heads/main/openapi/microsoft-suite-teams-api-openapi.yml
- filename: microsoft-suite-users-api-openapi.yml
  format: yaml
  label: Microsoft Suite Users API
  slug: microsoft-suite-users-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/microsoft-suite/refs/heads/main/openapi/microsoft-suite-users-api-openapi.yml
auth_types:
- oauth2
description: ''
kind: authentication
layout: security
method: derived
name: Microsoft Suite Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
- clientCredentials
overview: Microsoft Suite secures its APIs with oauth2 across 1 declared security scheme, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode and clientCredentials flow(s).
provider_name: Microsoft Suite
provider_slug: microsoft-suite
scheme_count: 1
schemes:
- description: Microsoft identity platform (Microsoft Entra ID) OAuth 2.0
  flows:
  - authorizationUrl: https://login.microsoftonline.com/common/oauth2/v2.0/authorize
    flow: authorizationCode
    scopes: 7
    tokenUrl: https://login.microsoftonline.com/common/oauth2/v2.0/token
  - flow: clientCredentials
    scopes: 1
    tokenUrl: https://login.microsoftonline.com/common/oauth2/v2.0/token
  name: OAuth2
  sources:
  - openapi/microsoft-suite-openapi.yml
  type: oauth2
slug: microsoft-suite-authentication
source_filename: microsoft-suite-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/microsoft-suite-openapi.yml\nsummary:\n  types:\n  - oauth2\n  oauth2_flows:\n  - authorizationCode\n  - clientCredentials\nschemes:\n- name: OAuth2\n  type: oauth2\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://login.microsoftonline.com/common/oauth2/v2.0/authorize\n    tokenUrl: https://login.microsoftonline.com/common/oauth2/v2.0/token\n    scopes: 7\n  - flow: clientCredentials\n    tokenUrl: https://login.microsoftonline.com/common/oauth2/v2.0/token\n    scopes: 1\n  description: Microsoft identity platform (Microsoft Entra ID) OAuth 2.0\n  sources:\n  - openapi/microsoft-suite-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/microsoft-suite/refs/heads/main/authentication/microsoft-suite-authentication.yml
summary_line: oauth2 · 1 scheme
tags:
- Cloud
- Enterprise
- Productivity
- SaaS
---
