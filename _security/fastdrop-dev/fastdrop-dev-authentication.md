---
anonymous_access: false
api_key_in: []
api_specs:
- filename: fastdrop-dev-health-api-openapi.yml
  format: yaml
  label: FastDrop Health API
  slug: fastdrop-dev-health-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/fastdrop-dev/openapi/fastdrop-dev-health-api-openapi.yml
- filename: fastdrop-dev-mcp-api-openapi.yml
  format: yaml
  label: FastDrop MCP API
  slug: fastdrop-dev-mcp-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/fastdrop-dev/openapi/fastdrop-dev-mcp-api-openapi.yml
- filename: fastdrop-dev-subregistry-api-openapi.yml
  format: yaml
  label: FastDrop Subregistry API
  slug: fastdrop-dev-subregistry-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/fastdrop-dev/openapi/fastdrop-dev-subregistry-api-openapi.yml
auth_types: []
description: Authentication schemes as published on FastDrop pages
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Fastdrop Dev Authentication
name_suffix: Authentication
oauth_flows: []
overview: FastDrop declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: FastDrop
provider_slug: fastdrop-dev
scheme_count: 1
schemes:
- evidence: 'Google-OAuth-gated LLM gateway: verify a Google ID token'
  name: Google OAuth
  type: oauth2
slug: fastdrop-dev-authentication
source_filename: fastdrop-dev-authentication.yml
source_heading: Authentication Profile
source_url: https://fastdrop.dev/p/authenticated-multi-llm-agent
source_yaml: "generated: '2026-11-07'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://fastdrop.dev/p/authenticated-multi-llm-agent\nsources:\n- https://fastdrop.dev/p/authenticated-multi-llm-agent\n- https://fastdrop.dev/p/sidecar\n- https://fastdrop.dev/p/lamina\n- https://fastdrop.dev/p/studiomeyer-academy\ndescription: Authentication schemes as published on FastDrop pages\nschemes:\n- type: oauth2\n  name: Google OAuth\n  evidence: 'Google-OAuth-gated LLM gateway: verify a Google ID token'\ndocs: https://fastdrop.dev/p/authenticated-multi-llm-agent\n"
source_yaml_url: https://artifacts.apis.io/fastdrop-dev/authentication/fastdrop-dev-authentication.yml
summary_line: 1 scheme
tags:
- launch-board
- MCP
- AI-agents
- software-discovery
- free-service
---
