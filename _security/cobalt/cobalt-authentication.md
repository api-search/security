---
api_key_in:
- header
api_specs:
- filename: cobalt-api-openapi.yml
  format: yaml
  label: Cobalt API
  slug: cobalt-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cobalt/refs/heads/main/openapi/cobalt-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Cobalt Authentication
name_suffix: Authentication
oauth_flows: []
overview: Cobalt secures its APIs with apiKey across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Cobalt
provider_slug: cobalt
scheme_count: 2
schemes:
- description: API key for authentication. Found in Cobalt dashboard under Settings > Developer > Setup tab.
  in: header
  name: apiKey
  parameter: x-api-key
  sources:
  - openapi/cobalt-api-openapi.yml
  type: apiKey
- description: Session token generated via the Session Token endpoint.
  in: header
  name: sessionToken
  parameter: Authorization
  sources:
  - openapi/cobalt-api-openapi.yml
  type: apiKey
slug: cobalt-authentication
source_filename: cobalt-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/cobalt-api-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: apiKey\n  type: apiKey\n  in: header\n  parameter: x-api-key\n  description: API key for authentication. Found in Cobalt dashboard under Settings > Developer\n    > Setup tab.\n  sources:\n  - openapi/cobalt-api-openapi.yml\n- name: sessionToken\n  type: apiKey\n  in: header\n  parameter: Authorization\n  description: Session token generated via the Session Token endpoint.\n  sources:\n  - openapi/cobalt-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/cobalt/refs/heads/main/authentication/cobalt-authentication.yml
summary_line: apiKey · 2 schemes
tags:
- Automation
- Embedded iPaaS
- Integrations
---
