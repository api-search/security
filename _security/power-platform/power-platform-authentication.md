---
api_key_in: []
api_specs:
- filename: v1
  format: yaml
  label: Power Apps API
  slug: power-apps-api
  spec_type: OpenAPI
  url: https://api.powerapps.com/openapi/v1
- filename: v1
  format: yaml
  label: Power Automate API
  slug: power-automate-api
  spec_type: OpenAPI
  url: https://api.flow.microsoft.com/openapi/v1
- filename: swagger.json
  format: json
  label: Power BI REST API
  slug: power-bi-rest-api
  spec_type: OpenAPI
  url: https://api.powerbi.com/v1.0/myorg/swagger.json
- filename: power-platform-api-openapi.json
  format: json
  label: Power Platform Unified API
  slug: power-platform-unified-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/power-platform/refs/heads/main/openapi/power-platform-api-openapi.json
auth_types:
- http
- oauth2
description: ''
kind: authentication
layout: security
method: derived
name: Power Platform Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
- clientCredentials
overview: Microsoft Power Platform APIs secures its APIs with http and oauth2 across 2 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode and clientCredentials flow(s).
provider_name: Microsoft Power Platform APIs
provider_slug: power-platform
scheme_count: 2
schemes:
- description: Microsoft Entra ID OAuth 2.0 authentication. Register your application and obtain tokens via the Microsoft identity platform.
  flows:
  - authorizationUrl: https://login.microsoftonline.com/common/oauth2/v2.0/authorize
    flow: authorizationCode
    scopes: 1
    tokenUrl: https://login.microsoftonline.com/common/oauth2/v2.0/token
  - flow: clientCredentials
    scopes: 1
    tokenUrl: https://login.microsoftonline.com/{tenantId}/oauth2/v2.0/token
  name: oauth2
  sources:
  - openapi/power-platform-api-openapi.json
  type: oauth2
- bearerFormat: JWT
  description: Bearer token obtained from Microsoft Entra ID OAuth 2.0 flow.
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/power-platform-api-openapi.json
  type: http
slug: power-platform-authentication
source_filename: power-platform-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/power-platform-api-openapi.json\nsummary:\n  types:\n  - http\n  - oauth2\n  oauth2_flows:\n  - authorizationCode\n  - clientCredentials\nschemes:\n- name: oauth2\n  type: oauth2\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://login.microsoftonline.com/common/oauth2/v2.0/authorize\n    tokenUrl: https://login.microsoftonline.com/common/oauth2/v2.0/token\n    scopes: 1\n  - flow: clientCredentials\n    tokenUrl: https://login.microsoftonline.com/{tenantId}/oauth2/v2.0/token\n    scopes: 1\n  description: Microsoft Entra ID OAuth 2.0 authentication. Register your application and obtain\n    tokens via the Microsoft identity platform.\n  sources:\n  - openapi/power-platform-api-openapi.json\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  description: Bearer token obtained from Microsoft Entra ID OAuth 2.0 flow.\n  sources:\n  - openapi/power-platform-api-openapi.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/power-platform/refs/heads/main/authentication/power-platform-authentication.yml
summary_line: http/oauth2 · 2 schemes
tags:
- Business Applications
- Copilot Studio
- Dataverse
- Low-Code
- Microsoft
- No-Code
- Power Pages
- Power Platform
---
