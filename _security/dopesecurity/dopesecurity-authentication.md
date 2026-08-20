---
api_key_in: []
api_specs:
- filename: dopesecurity-authorization-api-openapi.yml
  format: yaml
  label: dope.security Authorization API
  slug: dopesecurity-authorization-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dopesecurity/refs/heads/main/openapi/dopesecurity-authorization-api-openapi.yml
- filename: dopesecurity-custom-categories-api-openapi.yml
  format: yaml
  label: dope.security Custom Categories API
  slug: dopesecurity-custom-categories-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dopesecurity/refs/heads/main/openapi/dopesecurity-custom-categories-api-openapi.yml
- filename: dopesecurity-endpoints-api-openapi.yml
  format: yaml
  label: dope.security Endpoints API
  slug: dopesecurity-endpoints-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dopesecurity/refs/heads/main/openapi/dopesecurity-endpoints-api-openapi.yml
- filename: dopesecurity-policies-api-openapi.yml
  format: yaml
  label: dope.security Policies API
  slug: dopesecurity-policies-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dopesecurity/refs/heads/main/openapi/dopesecurity-policies-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Dopesecurity Authentication
name_suffix: Authentication
oauth_flows: []
overview: dope.security secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: dope.security
provider_slug: dopesecurity
scheme_count: 1
schemes:
- bearerFormat: JWT
  name: BearerAuth
  scheme: bearer
  sources:
  - openapi/dopesecurity-flightdeck-openapi.yml
  type: http
slug: dopesecurity-authentication
source_filename: dopesecurity-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: derived\nsource: openapi/dopesecurity-flightdeck-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: BearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  sources:\n  - openapi/dopesecurity-flightdeck-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/dopesecurity/refs/heads/main/authentication/dopesecurity-authentication.yml
summary_line: http · 1 scheme
tags:
- Company
- Enterprise
- Security
- Cybersecurity
- Secure Web Gateway
- SASE
- SSE
- Data Loss Prevention
- CASB
- Endpoint Security
---
