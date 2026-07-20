---
api_key_in:
- header
api_specs:
- filename: greenspark-openapi.yml
  format: yaml
  label: Greenspark Climate API
  slug: greenspark-climate-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/greenspark/refs/heads/main/openapi/greenspark-openapi.yml
auth_types:
- apiKey
description: 'Greenspark authenticates every API call with a single API key sent in the x-api-key request header. Keys are created in the Greenspark dashboard and are environment-bound: a sandbox key only works against the sandbox host and a production key only against production. No OAuth2/OIDC is offered.'
kind: authentication
layout: security
method: searched
name: Greenspark Authentication
name_suffix: Authentication
oauth_flows: []
overview: Greenspark secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Greenspark
provider_slug: greenspark
scheme_count: 1
schemes:
- description: 'Greenspark API key. Match key to host: sandbox key -> sandbox host, production key -> production host.'
  in: header
  name: ApiKeyAuth
  parameter: x-api-key
  sources:
  - openapi/greenspark-openapi.yml
  type: apiKey
slug: greenspark-authentication
source_filename: greenspark-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: searched\nsource: openapi/greenspark-openapi.yml\ndocs: https://docs.getgreenspark.com/docs/mcp\ndescription: >-\n  Greenspark authenticates every API call with a single API key sent in the\n  x-api-key request header. Keys are created in the Greenspark dashboard and are\n  environment-bound: a sandbox key only works against the sandbox host and a\n  production key only against production. No OAuth2/OIDC is offered.\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: ApiKeyAuth\n  type: apiKey\n  in: header\n  parameter: x-api-key\n  description: 'Greenspark API key. Match key to host: sandbox key -> sandbox host, production\n    key -> production host.'\n  sources:\n  - openapi/greenspark-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/greenspark/refs/heads/main/authentication/greenspark-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Sustainability
- Carbon Offset
- Climate
- Impact
- Carbon Estimation
- Reporting
- ESG
- Fintech
---
