---
anonymous_access: false
api_key_in:
- header
api_specs:
- filename: synapselayer-org-discovery-api-openapi.yml
  format: yaml
  label: Synapse Layer Discovery API
  slug: synapselayer-org-discovery-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/synapselayer-org/openapi/synapselayer-org-discovery-api-openapi.yml
- filename: synapselayer-org-memory-api-openapi.yml
  format: yaml
  label: Synapse Layer Memory API
  slug: synapselayer-org-memory-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/synapselayer-org/openapi/synapselayer-org-memory-api-openapi.yml
- filename: synapselayer-org-onboarding-api-openapi.yml
  format: yaml
  label: Synapse Layer Onboarding API
  slug: synapselayer-org-onboarding-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/synapselayer-org/openapi/synapselayer-org-onboarding-api-openapi.yml
- filename: synapselayer-org-operational-api-openapi.yml
  format: yaml
  label: Synapse Layer Operational API
  slug: synapselayer-org-operational-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/synapselayer-org/openapi/synapselayer-org-operational-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: derived
name: Synapse Layer Authentication
name_suffix: Authentication
oauth_flows: []
overview: Synapse Layer secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Synapse Layer
provider_slug: synapselayer-org
scheme_count: 1
schemes:
- description: 'Connect token (sk_connect_...). Also accepted as Authorization: Bearer <token>.'
  in: header
  name: connectToken
  parameter: x-connect-token
  sources:
  - openapi/forge-synapselayer-org-openapi.json
  - openapi/synapselayer-org-openapi.json
  type: apiKey
slug: synapselayer-org-authentication
source_filename: synapselayer-org-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-25'\nmethod: derived\nsource: openapi/forge-synapselayer-org-openapi.json, openapi/synapselayer-org-openapi.json\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: connectToken\n  type: apiKey\n  in: header\n  parameter: x-connect-token\n  description: 'Connect token (sk_connect_...). Also accepted as Authorization: Bearer <token>.'\n  sources:\n  - openapi/forge-synapselayer-org-openapi.json\n  - openapi/synapselayer-org-openapi.json\n"
source_yaml_url: https://artifacts.apis.io/synapselayer-org/authentication/synapselayer-org-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- AI
- Memory
- Encryption
- MCP
- Trust
---
