---
api_key_in:
- header
api_specs:
- filename: pandium-pandium-openapi.yml
  format: yaml
  label: Pandium
  slug: pandium
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pandium/refs/heads/main/openapi/pandium-pandium-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Pandium Authentication
name_suffix: Authentication
oauth_flows: []
overview: Pandium secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Pandium
provider_slug: pandium
scheme_count: 1
schemes:
- description: API key generated from the Settings sidebar in the Pandium Integration Hub under the API Access tab. Pass as a Bearer token in the Authorization header.
  in: header
  name: apiKey
  parameter: Authorization
  sources:
  - openapi/pandium-pandium-openapi.yml
  type: apiKey
slug: pandium-authentication
source_filename: pandium-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/pandium-pandium-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: apiKey\n  type: apiKey\n  in: header\n  parameter: Authorization\n  description: API key generated from the Settings sidebar in the Pandium Integration Hub under\n    the API Access tab. Pass as a Bearer token in the Authorization header.\n  sources:\n  - openapi/pandium-pandium-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/pandium/refs/heads/main/authentication/pandium-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- B2B
- Hubs
- Integrations
- Workflows
---
