---
api_key_in: []
api_specs:
- filename: llms.txt
  format: yaml
  label: Benchling REST API
  slug: benchling-rest-api
  spec_type: OpenAPI
  url: https://docs.benchling.com/llms.txt
auth_types:
- http
- oauth2
description: ''
kind: authentication
layout: security
method: derived
name: Benchling Authentication
name_suffix: Authentication
oauth_flows:
- clientCredentials
overview: Benchling secures its APIs with http and oauth2 across 2 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the clientCredentials flow(s).
provider_name: Benchling
provider_slug: benchling
scheme_count: 2
schemes:
- description: Use issued API key for standard access to the API
  name: basicApiKeyAuth
  scheme: basic
  sources:
  - openapi/benchling-openapi.yaml
  type: http
- description: OAuth2 Client Credentials flow intended for service access
  flows:
  - flow: clientCredentials
    scopes: 0
    tokenUrl: /api/v2/token
  name: oAuth
  sources:
  - openapi/benchling-openapi.yaml
  type: oauth2
slug: benchling-authentication
source_filename: benchling-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/benchling-openapi.yaml\nsummary:\n  types:\n  - http\n  - oauth2\n  oauth2_flows:\n  - clientCredentials\nschemes:\n- name: basicApiKeyAuth\n  type: http\n  scheme: basic\n  description: Use issued API key for standard access to the API\n  sources:\n  - openapi/benchling-openapi.yaml\n- name: oAuth\n  type: oauth2\n  flows:\n  - flow: clientCredentials\n    tokenUrl: /api/v2/token\n    scopes: 0\n  description: OAuth2 Client Credentials flow intended for service access\n  sources:\n  - openapi/benchling-openapi.yaml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/benchling/refs/heads/main/authentication/benchling-authentication.yml
summary_line: http/oauth2 · 2 schemes
tags:
- Life Sciences
- Biotech
- R&D
- Molecular Biology
- Laboratory Information Management
- Electronic Lab Notebook
- Assay Management
- Inventory Management
- Sequence Management
- Experiment Workflows
- REST
- Webhooks
---
