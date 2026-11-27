---
anonymous_access: false
api_key_in:
- header
api_specs:
- filename: agentnexus-app-discovery-api-openapi.yml
  format: yaml
  label: Agent Nexus Discovery API
  slug: agentnexus-app-discovery-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/agentnexus-app/openapi/agentnexus-app-discovery-api-openapi.yml
- filename: agentnexus-app-keys-api-openapi.yml
  format: yaml
  label: Agent Nexus Keys API
  slug: agentnexus-app-keys-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/agentnexus-app/openapi/agentnexus-app-keys-api-openapi.yml
- filename: agentnexus-app-registry-api-openapi.yml
  format: yaml
  label: Agent Nexus Registry API
  slug: agentnexus-app-registry-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/agentnexus-app/openapi/agentnexus-app-registry-api-openapi.yml
- filename: agentnexus-app-reliability-api-openapi.yml
  format: yaml
  label: Agent Nexus Reliability API
  slug: agentnexus-app-reliability-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/agentnexus-app/openapi/agentnexus-app-reliability-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: derived
name: Agent Nexus Authentication
name_suffix: Authentication
oauth_flows: []
overview: Agent Nexus secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Agent Nexus
provider_slug: agentnexus-app
scheme_count: 1
schemes:
- description: Optional. Free key raises the quota from 100 to 1,000 calls/day; Agent Pro 50,000/day.
  in: header
  name: apiKey
  parameter: x-api-key
  sources:
  - openapi/agentnexus-app-openapi.yml
  type: apiKey
slug: agentnexus-app-authentication
source_filename: agentnexus-app-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-15'\nmethod: derived\nsource: openapi/agentnexus-app-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: apiKey\n  type: apiKey\n  in: header\n  parameter: x-api-key\n  description: Optional. Free key raises the quota from 100 to 1,000 calls/day; Agent Pro 50,000/day.\n  sources:\n  - openapi/agentnexus-app-openapi.yml\n"
source_yaml_url: https://artifacts.apis.io/agentnexus-app/authentication/agentnexus-app-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Company
- Artificial Intelligence
- Infrastructure
- Registry
- Agents
- Platform
---
