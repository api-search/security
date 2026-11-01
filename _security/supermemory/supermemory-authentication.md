---
anonymous_access: false
api_key_in: []
api_specs:
- filename: supermemory-openapi.json
  format: json
  label: Supermemory API
  slug: supermemory-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/supermemory/openapi/supermemory-openapi.json
auth_types: []
description: Authentication schemes for Supermemory API
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Supermemory Authentication
name_suffix: Authentication
oauth_flows: []
overview: Supermemory declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: Supermemory
provider_slug: supermemory
scheme_count: 1
schemes:
- evidence: All API requests require authentication using a Bearer token.
  header: Authorization
  how_to_obtain: Get your API key from the Developer Platform.
  location: header
  name: Bearer
  type: http-bearer
slug: supermemory-authentication
source_filename: supermemory-authentication.yml
source_heading: Authentication Profile
source_url: https://supermemory.ai/docs/authentication
source_yaml: "generated: '2026-10-19'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://supermemory.ai/docs/authentication\nsources:\n- https://supermemory.ai/docs/authentication\n- https://supermemory.ai/docs/agents-and-mcp\n- https://supermemory.ai/docs/quickstart\ndescription: Authentication schemes for Supermemory API\nschemes:\n- type: http-bearer\n  name: Bearer\n  evidence: All API requests require authentication using a Bearer token.\n  location: header\n  header: Authorization\n  how_to_obtain: Get your API key from the Developer Platform.\nnote: No OAuth2, API key query, or other authentication methods are documented on the provided pages.\ndocs: https://supermemory.ai/docs/authentication\n"
source_yaml_url: https://artifacts.apis.io/supermemory/authentication/supermemory-authentication.yml
summary_line: 1 scheme
tags:
- Company
- Artificial Intelligence
- Memory
- Agents
- Platform
---
