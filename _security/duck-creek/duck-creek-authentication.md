---
api_key_in: []
api_specs:
- filename: duck-creek-policy-openapi.yml
  format: yaml
  label: Duck Creek Anywhere REST API
  slug: duck-creek-anywhere-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/duck-creek/refs/heads/main/openapi/duck-creek-policy-openapi.yml
- filename: duck-creek-policy-openapi.yml
  format: yaml
  label: Duck Creek Policy Administration API
  slug: duck-creek-policy-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/duck-creek/refs/heads/main/openapi/duck-creek-policy-openapi.yml
auth_types:
- oauth2
description: ''
kind: authentication
layout: security
method: derived
name: Duck Creek Authentication
name_suffix: Authentication
oauth_flows:
- clientCredentials
overview: duck-creek secures its APIs with oauth2 across 1 declared security scheme, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the clientCredentials flow(s).
provider_name: duck-creek
provider_slug: duck-creek
scheme_count: 1
schemes:
- description: OAuth 2.0 for Duck Creek Anywhere API authentication
  flows:
  - flow: clientCredentials
    scopes: 5
    tokenUrl: https://api.duckcreek.com/oauth/token
  name: oauth2
  sources:
  - openapi/duck-creek-policy-openapi.yml
  type: oauth2
slug: duck-creek-authentication
source_filename: duck-creek-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/duck-creek-policy-openapi.yml\nsummary:\n  types:\n  - oauth2\n  oauth2_flows:\n  - clientCredentials\nschemes:\n- name: oauth2\n  type: oauth2\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://api.duckcreek.com/oauth/token\n    scopes: 5\n  description: OAuth 2.0 for Duck Creek Anywhere API authentication\n  sources:\n  - openapi/duck-creek-policy-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/duck-creek/refs/heads/main/authentication/duck-creek-authentication.yml
summary_line: oauth2 · 1 scheme
tags: []
---
