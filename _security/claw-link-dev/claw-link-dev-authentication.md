---
anonymous_access: false
api_key_in: []
api_specs:
- filename: claw-link-dev-discovery-api-openapi.yml
  format: yaml
  label: ClawLink Discovery API
  slug: claw-link-dev-discovery-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/claw-link-dev/openapi/claw-link-dev-discovery-api-openapi.yml
- filename: claw-link-dev-execution-api-openapi.yml
  format: yaml
  label: ClawLink Execution API
  slug: claw-link-dev-execution-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/claw-link-dev/openapi/claw-link-dev-execution-api-openapi.yml
- filename: claw-link-dev-mcp-api-openapi.yml
  format: yaml
  label: ClawLink MCP API
  slug: claw-link-dev-mcp-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/claw-link-dev/openapi/claw-link-dev-mcp-api-openapi.yml
- filename: claw-link-dev-registration-api-openapi.yml
  format: yaml
  label: ClawLink Registration API
  slug: claw-link-dev-registration-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/claw-link-dev/openapi/claw-link-dev-registration-api-openapi.yml
auth_types: []
description: Authentication schemes for ClawLink Developer API
kind: authentication
layout: security
mechanism_count: 2
method: searched
name: ClawLink Authentication
name_suffix: Authentication
oauth_flows: []
overview: ClawLink declares 2 security scheme(s) across its OpenAPI definitions.
provider_name: ClawLink
provider_slug: claw-link-dev
scheme_count: 2
schemes:
- evidence: Every Developer API request authenticates with a ClawLink API key.
  header: Authorization
  how_to_obtain: Create a key in the ClawLink dashboard under Settings → Developer → Manual key.
  location: header
  name: ClawLink API key (Authorization header)
  type: apiKey
- evidence: 'Pass the key on every request using either of these headers: Authorization (Bearer) x-clawlink-api-key'
  header: x-clawlink-api-key
  how_to_obtain: Create a key in the ClawLink dashboard under Settings → Developer → Manual key.
  location: header
  name: ClawLink API key (x-clawlink-api-key header)
  type: apiKey
slug: claw-link-dev-authentication
source_filename: claw-link-dev-authentication.yml
source_heading: Authentication Profile
source_url: https://docs.claw-link.dev/api/authentication
source_yaml: "generated: '2026-11-04'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://docs.claw-link.dev/api/authentication\nsources:\n- https://docs.claw-link.dev/api/authentication\ndescription: Authentication schemes for ClawLink Developer API\nschemes:\n- type: apiKey\n  name: ClawLink API key (Authorization header)\n  evidence: Every Developer API request authenticates with a ClawLink API key.\n  location: header\n  header: Authorization\n  how_to_obtain: Create a key in the ClawLink dashboard under Settings → Developer → Manual key.\n- type: apiKey\n  name: ClawLink API key (x-clawlink-api-key header)\n  evidence: 'Pass the key on every request using either of these headers: Authorization (Bearer) x-clawlink-api-key'\n  location: header\n  header: x-clawlink-api-key\n  how_to_obtain: Create a key in the ClawLink dashboard under Settings → Developer → Manual key.\nnote: No OAuth2 or other authentication schemes are documented on the page.\ndocs: https://docs.claw-link.dev/api/authentication\n"
source_yaml_url: https://artifacts.apis.io/claw-link-dev/authentication/claw-link-dev-authentication.yml
summary_line: 2 schemes
tags:
- Artificial Intelligence
- Integration
- Automation
- Productivity
- Developer Tools
---
