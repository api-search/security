---
api_key_in:
- header
api_specs:
- filename: cycloid-cloudcost-api-openapi.yml
  format: yaml
  label: Cycloid CloudCost API
  slug: cycloid-cloudcost-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cycloid/refs/heads/main/openapi/cycloid-cloudcost-api-openapi.yml
- filename: cycloid-configrepositories-api-openapi.yml
  format: yaml
  label: Cycloid ConfigRepositories API
  slug: cycloid-configrepositories-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cycloid/refs/heads/main/openapi/cycloid-configrepositories-api-openapi.yml
- filename: cycloid-credentials-api-openapi.yml
  format: yaml
  label: Cycloid Credentials API
  slug: cycloid-credentials-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cycloid/refs/heads/main/openapi/cycloid-credentials-api-openapi.yml
- filename: cycloid-inventory-api-openapi.yml
  format: yaml
  label: Cycloid Inventory API
  slug: cycloid-inventory-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cycloid/refs/heads/main/openapi/cycloid-inventory-api-openapi.yml
- filename: cycloid-organizations-api-openapi.yml
  format: yaml
  label: Cycloid Organizations API
  slug: cycloid-organizations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cycloid/refs/heads/main/openapi/cycloid-organizations-api-openapi.yml
- filename: cycloid-pipelines-api-openapi.yml
  format: yaml
  label: Cycloid Pipelines API
  slug: cycloid-pipelines-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cycloid/refs/heads/main/openapi/cycloid-pipelines-api-openapi.yml
- filename: cycloid-projects-api-openapi.yml
  format: yaml
  label: Cycloid Projects API
  slug: cycloid-projects-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cycloid/refs/heads/main/openapi/cycloid-projects-api-openapi.yml
- filename: cycloid-servicecatalogs-api-openapi.yml
  format: yaml
  label: Cycloid ServiceCatalogs API
  slug: cycloid-servicecatalogs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cycloid/refs/heads/main/openapi/cycloid-servicecatalogs-api-openapi.yml
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
