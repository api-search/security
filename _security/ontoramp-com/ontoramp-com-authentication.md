---
anonymous_access: false
api_key_in: []
api_specs:
- filename: ontoramp-com-commerce-api-openapi.yml
  format: yaml
  label: ontoramp-com Commerce API
  slug: ontoramp-com-commerce-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/ontoramp-com/openapi/ontoramp-com-commerce-api-openapi.yml
- filename: ontoramp-com-decision-intelligence-api-openapi.yml
  format: yaml
  label: ontoramp-com Decision Intelligence API
  slug: ontoramp-com-decision-intelligence-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/ontoramp-com/openapi/ontoramp-com-decision-intelligence-api-openapi.yml
- filename: ontoramp-com-governance-evaluator-api-openapi.yml
  format: yaml
  label: ontoramp-com Governance Evaluator API
  slug: ontoramp-com-governance-evaluator-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/ontoramp-com/openapi/ontoramp-com-governance-evaluator-api-openapi.yml
- filename: ontoramp-com-knowledge-graph-api-openapi.yml
  format: yaml
  label: ontoramp-com Knowledge Graph API
  slug: ontoramp-com-knowledge-graph-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/ontoramp-com/openapi/ontoramp-com-knowledge-graph-api-openapi.yml
- filename: ontoramp-com-projection-engine-api-openapi.yml
  format: yaml
  label: ontoramp-com Projection Engine API
  slug: ontoramp-com-projection-engine-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/ontoramp-com/openapi/ontoramp-com-projection-engine-api-openapi.yml
auth_types: []
description: Authentication for OntoRamp MCP API
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Ontoramp Com Authentication
name_suffix: Authentication
oauth_flows: []
overview: ontoramp-com declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: ontoramp-com
provider_slug: ontoramp-com
scheme_count: 1
schemes:
- evidence: Every request is authenticated with an OntoRamp API key, presented as an HTTP Bearer token.
  header: Authorization
  how_to_obtain: Register a key on the MCP plugin hub (https://ontoramp.com/mcp) and use the displayed API key.
  location: header
  name: Bearer
  scopes:
  - read
  - read+write
  type: http-bearer
slug: ontoramp-com-authentication
source_filename: ontoramp-com-authentication.yml
source_heading: Authentication Profile
source_url: https://ontoramp.com/docs/agent-authentication
source_yaml: "generated: '2026-10-29'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://ontoramp.com/docs/agent-authentication\nsources:\n- https://ontoramp.com/docs/agent-authentication\n- https://ontoramp.com/docs/rfc-9728-discovery\n- https://ontoramp.com/docs/quickstart\n- https://ontoramp.com/docs/connect\ndescription: Authentication for OntoRamp MCP API\nschemes:\n- type: http-bearer\n  name: Bearer\n  evidence: Every request is authenticated with an OntoRamp API key, presented as an HTTP Bearer token.\n  location: header\n  header: Authorization\n  scopes:\n  - read\n  - read+write\n  how_to_obtain: Register a key on the MCP plugin hub (https://ontoramp.com/mcp) and use the displayed API key.\nnote: No OAuth2 flows are used; the server does not run an OAuth authorization server.\ndocs: https://ontoramp.com/docs/agent-authentication\n"
source_yaml_url: https://artifacts.apis.io/ontoramp-com/authentication/ontoramp-com-authentication.yml
summary_line: 1 scheme
tags:
- Company
- AI Governance
- Agentic AI
- Compliance
- Certification
---
