---
api_key_in: []
api_specs:
- filename: nav-webservices.yaml
  format: yaml
  label: Dynamics NAV Web Services API
  slug: dynamics-nav-web-services-api
  spec_type: OpenAPI
  url: https://example.com/openapi/nav-webservices.yaml
- filename: nav-odata.yaml
  format: yaml
  label: Dynamics NAV OData API
  slug: dynamics-nav-odata-api
  spec_type: OpenAPI
  url: https://example.com/openapi/nav-odata.yaml
- filename: business-central-api-v2.yml
  format: yaml
  label: Business Central API v2.0
  slug: business-central-api-v20
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/navision/refs/heads/main/openapi/business-central-api-v2.yml
- filename: admin-center-api.yml
  format: yaml
  label: Business Central Administration Center API
  slug: business-central-administration-center-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/navision/refs/heads/main/openapi/admin-center-api.yml
- filename: automation-api.yml
  format: yaml
  label: Business Central Automation API
  slug: business-central-automation-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/navision/refs/heads/main/openapi/automation-api.yml
auth_types:
- http
- oauth2
description: ''
kind: authentication
layout: security
method: derived
name: Navision Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
- clientCredentials
overview: Microsoft Dynamics NAV secures its APIs with http and oauth2 across 2 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode and clientCredentials flow(s).
provider_name: Microsoft Dynamics NAV
provider_slug: navision
scheme_count: 2
schemes:
- description: OAuth 2.0 authentication via Microsoft Entra ID
  flows:
  - authorizationUrl: https://login.microsoftonline.com/{tenantId}/oauth2/v2.0/authorize
    flow: authorizationCode
    scopes: 1
    tokenUrl: https://login.microsoftonline.com/{tenantId}/oauth2/v2.0/token
  - flow: clientCredentials
    scopes: 1
    tokenUrl: https://login.microsoftonline.com/{tenantId}/oauth2/v2.0/token
  name: oauth2
  sources:
  - openapi/admin-center-api.yml
  - openapi/automation-api.yml
  - openapi/business-central-api-v2.yml
  type: oauth2
- bearerFormat: JWT
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/admin-center-api.yml
  - openapi/automation-api.yml
  - openapi/business-central-api-v2.yml
  type: http
slug: navision-authentication
source_filename: navision-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/admin-center-api.yml, openapi/automation-api.yml, openapi/business-central-api-v2.yml\nsummary:\n  types:\n  - http\n  - oauth2\n  oauth2_flows:\n  - authorizationCode\n  - clientCredentials\nschemes:\n- name: oauth2\n  type: oauth2\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://login.microsoftonline.com/{tenantId}/oauth2/v2.0/authorize\n    tokenUrl: https://login.microsoftonline.com/{tenantId}/oauth2/v2.0/token\n    scopes: 1\n  - flow: clientCredentials\n    tokenUrl: https://login.microsoftonline.com/{tenantId}/oauth2/v2.0/token\n    scopes: 1\n  description: OAuth 2.0 authentication via Microsoft Entra ID\n  sources:\n  - openapi/admin-center-api.yml\n  - openapi/automation-api.yml\n  - openapi/business-central-api-v2.yml\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  sources:\n  - openapi/admin-center-api.yml\n  - openapi/automation-api.yml\n  - openapi/business-central-api-v2.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/navision/refs/heads/main/authentication/navision-authentication.yml
summary_line: http/oauth2 · 2 schemes
tags:
- Business Management
- Dynamics NAV
- ERP
- Finance
- Inventory
- Microsoft
- Navision
---
