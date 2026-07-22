---
api_key_in:
- header
api_specs:
- filename: rhizome-ai-openapi.yml
  format: yaml
  label: Rhizome AI API
  slug: rhizome-ai-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/rhizome-ai/refs/heads/main/openapi/rhizome-ai-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: searched
name: Rhizome Ai Authentication
name_suffix: Authentication
oauth_flows: []
overview: Rhizome Ai secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Rhizome Ai
provider_slug: rhizome-ai
scheme_count: 1
schemes:
- description: API key authentication. Create a key at https://rhizomeai.com/api-keys and send it in the x-api-key header. API access requires an enterprise plan.
  in: header
  name: apiKeyAuth
  parameter: x-api-key
  sources:
  - openapi/rhizome-ai-openapi.yml
  type: apiKey
slug: rhizome-ai-authentication
source_filename: rhizome-ai-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: searched\nsource: openapi/rhizome-ai-openapi.yml\ndocs: https://docs.rhizomeai.com/authentication\nnotes: >-\n  Single API-key scheme. Send the key in the x-api-key header on every request.\n  Create keys at https://rhizomeai.com/api-keys (shown once). API access\n  requires an enterprise plan. No test/live key distinction is documented.\n  Store keys in environment variables; never expose them in browser JavaScript.\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: apiKeyAuth\n  type: apiKey\n  in: header\n  parameter: x-api-key\n  description: API key authentication. Create a key at https://rhizomeai.com/api-keys and send\n    it in the x-api-key header. API access requires an enterprise plan.\n  sources:\n  - openapi/rhizome-ai-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/rhizome-ai/refs/heads/main/authentication/rhizome-ai-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Company
- Regulatory
- Pharmaceutical
- Medical Devices
- Life Sciences
- Document Search
- Artificial Intelligence
- Compliance
---
