---
api_key_in: []
api_specs:
- filename: accelo-openapi.yml
  format: yaml
  label: Accelo REST API
  slug: accelo-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/accelo/refs/heads/main/openapi/accelo-openapi.yml
auth_types:
- oauth2
description: ''
kind: authentication
layout: security
method: derived
name: Accelo Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
- clientCredentials
overview: Accelo secures its APIs with oauth2 across 1 declared security scheme, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode and clientCredentials flow(s).
provider_name: Accelo
provider_slug: accelo
scheme_count: 1
schemes:
- flows:
  - authorizationUrl: https://{deployment}.api.accelo.com/oauth2/v0/authorize
    flow: authorizationCode
    scopes: 0
    tokenUrl: https://{deployment}.api.accelo.com/oauth2/v0/token
  - flow: clientCredentials
    scopes: 0
    tokenUrl: https://{deployment}.api.accelo.com/oauth2/v0/token
  name: OAuth2
  sources:
  - openapi/accelo-openapi.yml
  type: oauth2
slug: accelo-authentication
source_filename: accelo-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/accelo-openapi.yml\nsummary:\n  types:\n  - oauth2\n  oauth2_flows:\n  - authorizationCode\n  - clientCredentials\nschemes:\n- name: OAuth2\n  type: oauth2\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://{deployment}.api.accelo.com/oauth2/v0/authorize\n    tokenUrl: https://{deployment}.api.accelo.com/oauth2/v0/token\n    scopes: 0\n  - flow: clientCredentials\n    tokenUrl: https://{deployment}.api.accelo.com/oauth2/v0/token\n    scopes: 0\n  sources:\n  - openapi/accelo-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/accelo/refs/heads/main/authentication/accelo-authentication.yml
summary_line: oauth2 · 1 scheme
tags:
- Professional Services Automation
- Project Management
- CRM
- Time Tracking
- Invoicing
- Service Operations
---
