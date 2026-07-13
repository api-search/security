---
api_key_in: []
api_specs:
- filename: openapi.json
  format: json
  label: Workday Extend REST API
  slug: workday-extend-rest-api
  spec_type: OpenAPI
  url: https://api.workday.com/extend/openapi.json
- filename: workday-extend-orchestration-openapi.yml
  format: yaml
  label: Workday Orchestration API
  slug: workday-orchestration-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/workday-extend/refs/heads/main/openapi/workday-extend-orchestration-openapi.yml
- filename: workday-extend-custom-objects-openapi.yml
  format: yaml
  label: Workday Custom Objects API
  slug: workday-custom-objects-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/workday-extend/refs/heads/main/openapi/workday-extend-custom-objects-openapi.yml
- filename: workday-extend-graph-api-openapi.yml
  format: yaml
  label: Workday Graph API
  slug: workday-graph-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/workday-extend/refs/heads/main/openapi/workday-extend-graph-api-openapi.yml
auth_types:
- oauth2
description: ''
kind: authentication
layout: security
method: derived
name: Workday Extend Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: Workday Extend secures its APIs with oauth2 across 1 declared security scheme, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: Workday Extend
provider_slug: workday-extend
scheme_count: 1
schemes:
- flows:
  - authorizationUrl: https://{baseUrl}/authorize
    flow: authorizationCode
    scopes: 2
    tokenUrl: https://{baseUrl}/oauth2/{tenant}/token
  name: OAuth2
  sources:
  - openapi/workday-extend-custom-objects-openapi.yml
  - openapi/workday-extend-graph-api-openapi.yml
  - openapi/workday-extend-orchestration-openapi.yml
  - openapi/workday-extend-rest-api-openapi.yml
  type: oauth2
slug: workday-extend-authentication
source_filename: workday-extend-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/workday-extend-custom-objects-openapi.yml, openapi/workday-extend-graph-api-openapi.yml,\n  openapi/workday-extend-orchestration-openapi.yml, openapi/workday-extend-rest-api-openapi.yml\nsummary:\n  types:\n  - oauth2\n  oauth2_flows:\n  - authorizationCode\nschemes:\n- name: OAuth2\n  type: oauth2\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://{baseUrl}/authorize\n    tokenUrl: https://{baseUrl}/oauth2/{tenant}/token\n    scopes: 2\n  sources:\n  - openapi/workday-extend-custom-objects-openapi.yml\n  - openapi/workday-extend-graph-api-openapi.yml\n  - openapi/workday-extend-orchestration-openapi.yml\n  - openapi/workday-extend-rest-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/workday-extend/refs/heads/main/authentication/workday-extend-authentication.yml
summary_line: oauth2 · 1 scheme
tags:
- Automation
- Custom Applications
- Enterprise
- Extensions
- HCM
- Human Capital Management
- Integration
- Orchestration
- PaaS
---
