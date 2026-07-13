---
api_key_in:
- header
api_specs:
- filename: nuix-nuix-core-engine-rest-api-openapi.yml
  format: yaml
  label: Nuix Core Engine REST API
  slug: nuix-core-engine-rest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nuix/refs/heads/main/openapi/nuix-nuix-core-engine-rest-api-openapi.yml
- filename: nuix-nuix-ecc-rest-api-openapi.yml
  format: yaml
  label: Nuix Enterprise Collection Center REST API
  slug: nuix-ecc-rest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nuix/refs/heads/main/openapi/nuix-nuix-ecc-rest-api-openapi.yml
auth_types:
- apiKey
- http
description: ''
kind: authentication
layout: security
method: derived
name: Nuix Authentication
name_suffix: Authentication
oauth_flows: []
overview: Nuix secures its APIs with apiKey and http across 3 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Nuix
provider_slug: nuix
scheme_count: 3
schemes:
- in: header
  name: ApiKeyAuth
  parameter: nuix-auth-token
  sources:
  - openapi/nuix-nuix-core-engine-rest-api-openapi.yml
  type: apiKey
- bearerFormat: JWT
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/nuix-nuix-core-engine-rest-api-openapi.yml
  type: http
- name: BasicAuth
  scheme: basic
  sources:
  - openapi/nuix-nuix-ecc-rest-api-openapi.yml
  type: http
slug: nuix-authentication
source_filename: nuix-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/nuix-nuix-core-engine-rest-api-openapi.yml, openapi/nuix-nuix-ecc-rest-api-openapi.yml\nsummary:\n  types:\n  - apiKey\n  - http\n  api_key_in:\n  - header\nschemes:\n- name: ApiKeyAuth\n  type: apiKey\n  in: header\n  parameter: nuix-auth-token\n  sources:\n  - openapi/nuix-nuix-core-engine-rest-api-openapi.yml\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  sources:\n  - openapi/nuix-nuix-core-engine-rest-api-openapi.yml\n- name: BasicAuth\n  type: http\n  scheme: basic\n  sources:\n  - openapi/nuix-nuix-ecc-rest-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/nuix/refs/heads/main/authentication/nuix-authentication.yml
summary_line: apiKey/http · 3 schemes
tags:
- Forensics
- eDiscovery
- Investigations
- Compliance
- Data Processing
- Legal Technology
- Intelligence
---
