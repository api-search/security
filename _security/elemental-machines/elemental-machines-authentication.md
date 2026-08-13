---
api_key_in:
- query
api_specs:
- filename: elemental-machines-api-openapi.yml
  format: yaml
  label: Elemental Machines API
  slug: elemental-machines-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/elemental-machines/refs/heads/main/openapi/elemental-machines-api-openapi.yml
auth_types:
- apiKey
- oauth2
description: ''
kind: authentication
layout: security
method: derived
name: Elemental Machines Authentication
name_suffix: Authentication
oauth_flows:
- password
overview: Elemental Machines secures its APIs with apiKey and oauth2 across 2 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the password flow(s).
provider_name: Elemental Machines
provider_slug: elemental-machines
scheme_count: 2
schemes:
- description: OAuth 2.0 access token passed as the access_token query parameter. Obtain one from POST /oauth/token (Resource Owner Password Credentials grant).
  in: query
  name: access_token
  parameter: access_token
  sources:
  - openapi/elemental-machines-api-openapi.yml
  type: apiKey
- description: Resource Owner Password Credentials grant. Documented in the provider's Swagger 1.2 declaration at /docs/api/oauth.json.
  flows:
  - flow: password
    scopes: 0
    tokenUrl: https://api.elementalmachines.io/oauth/token
  name: oauth2_password
  sources:
  - openapi/elemental-machines-api-openapi.yml
  type: oauth2
slug: elemental-machines-authentication
source_filename: elemental-machines-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-12'\nmethod: derived\nsource: openapi/elemental-machines-api-openapi.yml\nsummary:\n  types:\n  - apiKey\n  - oauth2\n  api_key_in:\n  - query\n  oauth2_flows:\n  - password\nschemes:\n- name: access_token\n  type: apiKey\n  in: query\n  parameter: access_token\n  description: OAuth 2.0 access token passed as the access_token query parameter. Obtain one\n    from POST /oauth/token (Resource Owner Password Credentials grant).\n  sources:\n  - openapi/elemental-machines-api-openapi.yml\n- name: oauth2_password\n  type: oauth2\n  flows:\n  - flow: password\n    tokenUrl: https://api.elementalmachines.io/oauth/token\n    scopes: 0\n  description: Resource Owner Password Credentials grant. Documented in the provider's Swagger\n    1.2 declaration at /docs/api/oauth.json.\n  sources:\n  - openapi/elemental-machines-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/elemental-machines/refs/heads/main/authentication/elemental-machines-authentication.yml
summary_line: apiKey/oauth2 · 2 schemes
tags:
- lab-operations
- laboratory-monitoring
- iot
- sensors
- life-sciences
- cold-chain
- environmental-monitoring
- equipment-utilization
- asset-management
- alerting
- compliance
- gxp
- manufacturing
- time-series
---
