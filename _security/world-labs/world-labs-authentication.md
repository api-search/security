---
api_key_in:
- header
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: World Labs Authentication
name_suffix: Authentication
oauth_flows: []
overview: World Labs secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: World Labs
provider_slug: world-labs
scheme_count: 1
schemes:
- description: API key for authentication. Get your key from the developer portal.
  in: header
  name: ApiKeyAuth
  parameter: WLT-Api-Key
  sources:
  - openapi/world-labs-marble-openapi-original.yml
  type: apiKey
slug: world-labs-authentication
source_filename: world-labs-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: derived\nsource: openapi/world-labs-marble-openapi-original.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: ApiKeyAuth\n  type: apiKey\n  in: header\n  parameter: WLT-Api-Key\n  description: API key for authentication. Get your key from the developer portal.\n  sources:\n  - openapi/world-labs-marble-openapi-original.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/world-labs/refs/heads/main/authentication/world-labs-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Company
- Ai
---
