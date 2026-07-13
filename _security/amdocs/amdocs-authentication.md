---
api_key_in: []
api_specs:
- filename: amdocs-connectx-openapi.yml
  format: yaml
  label: Amdocs connectX BSS API
  slug: amdocs-connectx-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amdocs/refs/heads/main/openapi/amdocs-connectx-openapi.yml
auth_types:
- oauth2
description: ''
kind: authentication
layout: security
method: derived
name: Amdocs Authentication
name_suffix: Authentication
oauth_flows:
- clientCredentials
overview: Amdocs secures its APIs with oauth2 across 1 declared security scheme, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the clientCredentials flow(s).
provider_name: Amdocs
provider_slug: amdocs
scheme_count: 1
schemes:
- flows:
  - flow: clientCredentials
    scopes: 4
    tokenUrl: https://auth.amdocs-dbs.com/oauth/token
  name: oauth2
  sources:
  - openapi/amdocs-connectx-openapi.yml
  type: oauth2
slug: amdocs-authentication
source_filename: amdocs-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/amdocs-connectx-openapi.yml\nsummary:\n  types:\n  - oauth2\n  oauth2_flows:\n  - clientCredentials\nschemes:\n- name: oauth2\n  type: oauth2\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://auth.amdocs-dbs.com/oauth/token\n    scopes: 4\n  sources:\n  - openapi/amdocs-connectx-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/amdocs/refs/heads/main/authentication/amdocs-authentication.yml
summary_line: oauth2 · 1 scheme
tags:
- Telecom
- BSS
- OSS
- Billing
- Customer Management
- MVNO
- 5G
- SaaS
---
