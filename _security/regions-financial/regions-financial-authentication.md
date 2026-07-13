---
api_key_in: []
api_specs:
- filename: regions-open-banking-openapi.yml
  format: yaml
  label: Regions Open Banking API
  slug: regions-open-banking-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/regions-financial/refs/heads/main/openapi/regions-open-banking-openapi.yml
auth_types:
- oauth2
description: ''
kind: authentication
layout: security
method: derived
name: Regions Financial Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: regions-financial secures its APIs with oauth2 across 1 declared security scheme, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: regions-financial
provider_slug: regions-financial
scheme_count: 1
schemes:
- description: OAuth 2.0 with customer consent (FDX standard)
  flows:
  - authorizationUrl: https://auth.regions.com/oauth/authorize
    flow: authorizationCode
    scopes: 4
    tokenUrl: https://auth.regions.com/oauth/token
  name: OAuth2
  sources:
  - openapi/regions-open-banking-openapi.yml
  type: oauth2
slug: regions-financial-authentication
source_filename: regions-financial-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/regions-open-banking-openapi.yml\nsummary:\n  types:\n  - oauth2\n  oauth2_flows:\n  - authorizationCode\nschemes:\n- name: OAuth2\n  type: oauth2\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://auth.regions.com/oauth/authorize\n    tokenUrl: https://auth.regions.com/oauth/token\n    scopes: 4\n  description: OAuth 2.0 with customer consent (FDX standard)\n  sources:\n  - openapi/regions-open-banking-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/regions-financial/refs/heads/main/authentication/regions-financial-authentication.yml
summary_line: oauth2 · 1 scheme
tags:
- Banking
- Financial Services
- Open Banking
- FDX
- Consumer Banking
- Wealth Management
- Fortune 500
---
