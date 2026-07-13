---
api_key_in:
- header
api_specs:
- filename: cycloid-api-openapi.yml
  format: yaml
  label: Cycloid HTTP API
  slug: http-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cycloid/refs/heads/main/openapi/cycloid-api-openapi.yml
auth_types:
- apiKey
- oauth2
description: ''
kind: authentication
layout: security
method: derived
name: Cycloid Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: Cycloid secures its APIs with apiKey and oauth2 across 2 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: Cycloid
provider_slug: cycloid
scheme_count: 2
schemes:
- in: header
  name: ApiKeyAuth
  parameter: Authorization
  sources:
  - openapi/cycloid-api-openapi.yml
  type: apiKey
- flows:
  - authorizationUrl: https://console.cycloid.io/oauth/authorize
    flow: authorizationCode
    scopes: 2
    tokenUrl: https://http-api.cycloid.io/oauth/token
  name: OAuth2
  sources:
  - openapi/cycloid-api-openapi.yml
  type: oauth2
slug: cycloid-authentication
source_filename: cycloid-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/cycloid-api-openapi.yml\nsummary:\n  types:\n  - apiKey\n  - oauth2\n  api_key_in:\n  - header\n  oauth2_flows:\n  - authorizationCode\nschemes:\n- name: ApiKeyAuth\n  type: apiKey\n  in: header\n  parameter: Authorization\n  sources:\n  - openapi/cycloid-api-openapi.yml\n- name: OAuth2\n  type: oauth2\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://console.cycloid.io/oauth/authorize\n    tokenUrl: https://http-api.cycloid.io/oauth/token\n    scopes: 2\n  sources:\n  - openapi/cycloid-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/cycloid/refs/heads/main/authentication/cycloid-authentication.yml
summary_line: apiKey/oauth2 · 2 schemes
tags:
- Asset Inventory
- CI/CD
- Cloud Cost Management
- Cloud Management
- Developer Experience
- DevOps
- FinOps
- GitOps
- GreenOps
- Infrastructure as Code
- Internal Developer Platform
- Internal Developer Portal
- Multi-Cloud
- Platform Engineering
- RBAC
- Self-Service
- Service Catalog
- StackForms
- Terraform
---
