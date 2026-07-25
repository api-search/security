---
api_key_in:
- header
api_specs:
- filename: greenspark-account-api-openapi.yml
  format: yaml
  label: Greenspark Account API
  slug: greenspark-account-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/greenspark/refs/heads/main/openapi/greenspark-account-api-openapi.yml
- filename: greenspark-email-api-openapi.yml
  format: yaml
  label: Greenspark Email API
  slug: greenspark-email-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/greenspark/refs/heads/main/openapi/greenspark-email-api-openapi.yml
- filename: greenspark-estimations-api-openapi.yml
  format: yaml
  label: Greenspark Estimations API
  slug: greenspark-estimations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/greenspark/refs/heads/main/openapi/greenspark-estimations-api-openapi.yml
- filename: greenspark-impacts-api-openapi.yml
  format: yaml
  label: Greenspark Impacts API
  slug: greenspark-impacts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/greenspark/refs/heads/main/openapi/greenspark-impacts-api-openapi.yml
- filename: greenspark-projects-api-openapi.yml
  format: yaml
  label: Greenspark Projects API
  slug: greenspark-projects-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/greenspark/refs/heads/main/openapi/greenspark-projects-api-openapi.yml
- filename: greenspark-reports-api-openapi.yml
  format: yaml
  label: Greenspark Reports API
  slug: greenspark-reports-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/greenspark/refs/heads/main/openapi/greenspark-reports-api-openapi.yml
- filename: greenspark-widgets-api-openapi.yml
  format: yaml
  label: Greenspark Widgets API
  slug: greenspark-widgets-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/greenspark/refs/heads/main/openapi/greenspark-widgets-api-openapi.yml
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
