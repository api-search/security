---
api_key_in: []
api_specs:
- filename: state-farm-renters-insurance-openapi.yml
  format: yaml
  label: Renters Insurance API
  slug: renters-insurance-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/state-farm/refs/heads/main/openapi/state-farm-renters-insurance-openapi.yml
auth_types:
- oauth2
description: ''
kind: authentication
layout: security
method: derived
name: State Farm Authentication
name_suffix: Authentication
oauth_flows:
- clientCredentials
overview: State Farm secures its APIs with oauth2 across 1 declared security scheme, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the clientCredentials flow(s).
provider_name: State Farm
provider_slug: state-farm
scheme_count: 1
schemes:
- flows:
  - flow: clientCredentials
    scopes: 3
    tokenUrl: https://api.statefarm.com/oauth/token
  name: OAuth2
  sources:
  - openapi/state-farm-renters-insurance-openapi.yml
  type: oauth2
slug: state-farm-authentication
source_filename: state-farm-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/state-farm-renters-insurance-openapi.yml\nsummary:\n  types:\n  - oauth2\n  oauth2_flows:\n  - clientCredentials\nschemes:\n- name: OAuth2\n  type: oauth2\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://api.statefarm.com/oauth/token\n    scopes: 3\n  sources:\n  - openapi/state-farm-renters-insurance-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/state-farm/refs/heads/main/authentication/state-farm-authentication.yml
summary_line: oauth2 · 1 scheme
tags: []
---
