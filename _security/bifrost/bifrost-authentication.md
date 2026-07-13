---
api_key_in:
- header
api_specs:
- filename: bifrost-http-gateway-api.yaml
  format: yaml
  label: Bifrost HTTP Gateway API
  slug: bifrost-http-gateway-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bifrost/refs/heads/main/openapi/bifrost-http-gateway-api.yaml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Bifrost Authentication
name_suffix: Authentication
oauth_flows: []
overview: Bifrost secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Bifrost
provider_slug: bifrost
scheme_count: 1
schemes:
- description: Provider API key passed as x-bf-provider-key header. Alternatively, provider keys can be configured server-side in bifrost configuration.
  in: header
  name: BifrostProviderAuth
  parameter: x-bf-provider-key
  sources:
  - openapi/bifrost-http-gateway-api.yaml
  type: apiKey
slug: bifrost-authentication
source_filename: bifrost-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/bifrost-http-gateway-api.yaml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: BifrostProviderAuth\n  type: apiKey\n  in: header\n  parameter: x-bf-provider-key\n  description: Provider API key passed as x-bf-provider-key header. Alternatively, provider\n    keys can be configured server-side in bifrost configuration.\n  sources:\n  - openapi/bifrost-http-gateway-api.yaml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/bifrost/refs/heads/main/authentication/bifrost-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- AI Gateway
- LLM
- Load Balancing
- Open Source
- OpenAI Compatible
- MCP
---
