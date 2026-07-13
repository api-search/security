---
api_key_in:
- header
api_specs:
- filename: hotglue-openapi.yml
  format: yaml
  label: Hotglue API V2
  slug: hotglue-api-v2
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hotglue/refs/heads/main/openapi/hotglue-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Hotglue Authentication
name_suffix: Authentication
oauth_flows: []
overview: Hotglue secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Hotglue
provider_slug: hotglue
scheme_count: 1
schemes:
- in: header
  name: ApiKeyAuth
  parameter: x-api-key
  sources:
  - openapi/hotglue-openapi.yml
  type: apiKey
slug: hotglue-authentication
source_filename: hotglue-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/hotglue-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: ApiKeyAuth\n  type: apiKey\n  in: header\n  parameter: x-api-key\n  sources:\n  - openapi/hotglue-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/hotglue/refs/heads/main/authentication/hotglue-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Connectors
- Embedded Integrations
- ETL
- Integration Platform
- iPaaS
---
