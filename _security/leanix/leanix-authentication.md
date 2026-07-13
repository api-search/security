---
api_key_in: []
api_specs:
- filename: leanix-openapi.json
  format: json
  label: LeanIX Integration API
  slug: integration-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/leanix/refs/heads/main/openapi/leanix-openapi.json
auth_types:
- oauth2
description: ''
kind: authentication
layout: security
method: derived
name: Leanix Authentication
name_suffix: Authentication
oauth_flows:
- clientCredentials
overview: LeanIX secures its APIs with oauth2 across 1 declared security scheme, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the clientCredentials flow(s).
provider_name: LeanIX
provider_slug: leanix
scheme_count: 1
schemes:
- flows:
  - flow: clientCredentials
    scopes: 0
    tokenUrl: /services/mtm/v1/oauth2/token
  name: token
  sources:
  - openapi/leanix-openapi.json
  type: oauth2
slug: leanix-authentication
source_filename: leanix-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/leanix-openapi.json\nsummary:\n  types:\n  - oauth2\n  oauth2_flows:\n  - clientCredentials\nschemes:\n- name: token\n  type: oauth2\n  flows:\n  - flow: clientCredentials\n    tokenUrl: /services/mtm/v1/oauth2/token\n    scopes: 0\n  sources:\n  - openapi/leanix-openapi.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/leanix/refs/heads/main/authentication/leanix-authentication.yml
summary_line: oauth2 · 1 scheme
tags:
- Enterprise Architecture
- SaaS Management
- IT Portfolio Management
- Application Portfolio
- Technology Risk
---
