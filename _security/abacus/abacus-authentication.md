---
api_key_in: []
api_specs:
- filename: abacus-authentication-api-openapi.yml
  format: yaml
  label: Abacus Authentication API
  slug: abacus-authentication-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/abacus/refs/heads/main/openapi/abacus-authentication-api-openapi.yml
- filename: abacus-expenses-api-openapi.yml
  format: yaml
  label: Abacus Expenses API
  slug: abacus-expenses-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/abacus/refs/heads/main/openapi/abacus-expenses-api-openapi.yml
- filename: abacus-members-api-openapi.yml
  format: yaml
  label: Abacus Members API
  slug: abacus-members-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/abacus/refs/heads/main/openapi/abacus-members-api-openapi.yml
auth_types:
- oauth2
description: ''
kind: authentication
layout: security
method: derived
name: Abacus Authentication
name_suffix: Authentication
oauth_flows:
- clientCredentials
overview: Abacus secures its APIs with oauth2 across 1 declared security scheme, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the clientCredentials flow(s).
provider_name: Abacus
provider_slug: abacus
scheme_count: 1
schemes:
- description: OAuth 2.0 client credentials flow for API authentication
  flows:
  - flow: clientCredentials
    scopes: 3
    tokenUrl: https://api.abacus.com/oauth/token
  name: OAuth2
  sources:
  - openapi/abacus-api-openapi.yaml
  type: oauth2
slug: abacus-authentication
source_filename: abacus-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/abacus-api-openapi.yaml\nsummary:\n  types:\n  - oauth2\n  oauth2_flows:\n  - clientCredentials\nschemes:\n- name: OAuth2\n  type: oauth2\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://api.abacus.com/oauth/token\n    scopes: 3\n  description: OAuth 2.0 client credentials flow for API authentication\n  sources:\n  - openapi/abacus-api-openapi.yaml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/abacus/refs/heads/main/authentication/abacus-authentication.yml
summary_line: oauth2 · 1 scheme
tags:
- Accounting
- Expense Management
- Finance
- Reimbursement
---
