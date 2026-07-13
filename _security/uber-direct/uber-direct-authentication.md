---
api_key_in: []
api_specs:
- filename: uber-direct-openapi.yml
  format: yaml
  label: Uber Direct API
  slug: uber-direct-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/uber-direct/refs/heads/main/openapi/uber-direct-openapi.yml
auth_types:
- oauth2
description: ''
kind: authentication
layout: security
method: derived
name: Uber Direct Authentication
name_suffix: Authentication
oauth_flows:
- clientCredentials
overview: Uber Direct secures its APIs with oauth2 across 1 declared security scheme, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the clientCredentials flow(s).
provider_name: Uber Direct
provider_slug: uber-direct
scheme_count: 1
schemes:
- flows:
  - flow: clientCredentials
    scopes: 1
    tokenUrl: https://auth.uber.com/oauth/v2/token
  name: oauth2
  sources:
  - openapi/uber-direct-openapi.yml
  type: oauth2
slug: uber-direct-authentication
source_filename: uber-direct-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/uber-direct-openapi.yml\nsummary:\n  types:\n  - oauth2\n  oauth2_flows:\n  - clientCredentials\nschemes:\n- name: oauth2\n  type: oauth2\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://auth.uber.com/oauth/v2/token\n    scopes: 1\n  sources:\n  - openapi/uber-direct-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/uber-direct/refs/heads/main/authentication/uber-direct-authentication.yml
summary_line: oauth2 · 1 scheme
tags:
- Logistics
- Last Mile Delivery
- Couriers
- Fulfillment
- DaaS
---
