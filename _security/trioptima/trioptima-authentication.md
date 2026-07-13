---
api_key_in: []
api_specs:
- filename: trioptima-trireduce-api-openapi.yml
  format: yaml
  label: Trioptima triReduce API
  slug: trireduce-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/trioptima/refs/heads/main/openapi/trioptima-trireduce-api-openapi.yml
auth_types:
- oauth2
description: ''
kind: authentication
layout: security
method: derived
name: Trioptima Authentication
name_suffix: Authentication
oauth_flows:
- clientCredentials
overview: Trioptima secures its APIs with oauth2 across 1 declared security scheme, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the clientCredentials flow(s).
provider_name: Trioptima
provider_slug: trioptima
scheme_count: 1
schemes:
- flows:
  - flow: clientCredentials
    scopes: 2
    tokenUrl: https://auth.trireduce.com/oauth/token
  name: oauth2
  sources:
  - openapi/trioptima-trireduce-api-openapi.yml
  type: oauth2
slug: trioptima-authentication
source_filename: trioptima-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/trioptima-trireduce-api-openapi.yml\nsummary:\n  types:\n  - oauth2\n  oauth2_flows:\n  - clientCredentials\nschemes:\n- name: oauth2\n  type: oauth2\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://auth.trireduce.com/oauth/token\n    scopes: 2\n  sources:\n  - openapi/trioptima-trireduce-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/trioptima/refs/heads/main/authentication/trioptima-authentication.yml
summary_line: oauth2 · 1 scheme
tags:
- CME Group
- Derivatives
- Financial Services
- OSTTRA
- Portfolio Compression
- Post-Trade Services
- Reconciliation
- Risk Management
---
