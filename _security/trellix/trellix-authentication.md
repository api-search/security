---
api_key_in: []
api_specs:
- filename: trellix-epo-saas-openapi.yml
  format: yaml
  label: Trellix ePO SaaS API
  slug: trellix-epo-saas-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/trellix/refs/heads/main/openapi/trellix-epo-saas-openapi.yml
- filename: trellix-edr-openapi.yml
  format: yaml
  label: Trellix EDR API
  slug: trellix-edr-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/trellix/refs/heads/main/openapi/trellix-edr-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Trellix Authentication
name_suffix: Authentication
oauth_flows: []
overview: Trellix secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Trellix
provider_slug: trellix
scheme_count: 1
schemes:
- bearerFormat: JWT
  description: OAuth 2.0 access token obtained through the client credentials flow with soc.act.tg scope. Credentials are generated through the Trellix EDR Credential Generator.
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/trellix-edr-openapi.yml
  - openapi/trellix-epo-saas-openapi.yml
  type: http
slug: trellix-authentication
source_filename: trellix-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/trellix-edr-openapi.yml, openapi/trellix-epo-saas-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  description: OAuth 2.0 access token obtained through the client credentials flow with soc.act.tg\n    scope. Credentials are generated through the Trellix EDR Credential Generator.\n  sources:\n  - openapi/trellix-edr-openapi.yml\n  - openapi/trellix-epo-saas-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/trellix/refs/heads/main/authentication/trellix-authentication.yml
summary_line: http · 1 scheme
tags:
- Cloud Security
- Cybersecurity
- Endpoint Security
- Threat Detection
- Threat Intelligence
- XDR
---
