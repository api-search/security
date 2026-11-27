---
anonymous_access: false
api_key_in: []
api_specs:
- filename: agentsim-dev-agents-api-openapi.yml
  format: yaml
  label: AgentSIM Agents API
  slug: agentsim-dev-agents-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/agentsim-dev/openapi/agentsim-dev-agents-api-openapi.yml
- filename: agentsim-dev-browser-access-api-openapi.yml
  format: yaml
  label: AgentSIM Browser Access API
  slug: agentsim-dev-browser-access-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/agentsim-dev/openapi/agentsim-dev-browser-access-api-openapi.yml
- filename: agentsim-dev-sessions-api-openapi.yml
  format: yaml
  label: AgentSIM Sessions API
  slug: agentsim-dev-sessions-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/agentsim-dev/openapi/agentsim-dev-sessions-api-openapi.yml
auth_types: []
description: ''
kind: authentication
layout: security
mechanism_count: 2
method: searched
name: AgentSIM Authentication
name_suffix: Authentication
oauth_flows: []
overview: AgentSIM declares 2 security scheme(s) across its OpenAPI definitions.
provider_name: AgentSIM
provider_slug: agentsim-dev
scheme_count: 2
schemes:
- description: API key for challenge APIs
  in: header
  name: x-api-key
  type: apiKey
- bearerFormat: DPoP
  description: Runtime-bound bearer token for Browser Access, with Ed25519 DPoP proof
  scheme: bearer
  type: http
slug: agentsim-dev-authentication
source_filename: agentsim-dev-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-01'\nmethod: searched\nsource: https://docs.agentsim.dev/authentication.md\nschemes:\n  - type: apiKey\n    name: x-api-key\n    in: header\n    description: API key for challenge APIs\n  - type: http\n    scheme: bearer\n    bearerFormat: DPoP\n    description: Runtime-bound bearer token for Browser Access, with Ed25519 DPoP proof"
source_yaml_url: https://artifacts.apis.io/agentsim-dev/authentication/agentsim-dev-authentication.yml
summary_line: 2 schemes
tags:
- AgentSIM
- Authentication
- Identity
- Security
---
