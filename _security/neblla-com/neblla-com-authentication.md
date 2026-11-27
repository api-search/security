---
anonymous_access: false
api_key_in: []
api_specs:
- filename: neblla-com-connect-api-openapi.yml
  format: yaml
  label: Neblla Connect API
  slug: neblla-com-connect-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/neblla-com/openapi/neblla-com-connect-api-openapi.yml
- filename: neblla-com-gallery-api-openapi.yml
  format: yaml
  label: Neblla Gallery API
  slug: neblla-com-gallery-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/neblla-com/openapi/neblla-com-gallery-api-openapi.yml
- filename: neblla-com-llms-api-openapi.yml
  format: yaml
  label: Neblla Llms API
  slug: neblla-com-llms-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/neblla-com/openapi/neblla-com-llms-api-openapi.yml
- filename: neblla-com-llms-full-txt-api-openapi.yml
  format: yaml
  label: Neblla Llms Full.txt API
  slug: neblla-com-llms-full-txt-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/neblla-com/openapi/neblla-com-llms-full-txt-api-openapi.yml
- filename: neblla-com-llms-txt-api-openapi.yml
  format: yaml
  label: Neblla Llms.txt API
  slug: neblla-com-llms-txt-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/neblla-com/openapi/neblla-com-llms-txt-api-openapi.yml
- filename: neblla-com-mcp-api-openapi.yml
  format: yaml
  label: Neblla MCP API
  slug: neblla-com-mcp-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/neblla-com/openapi/neblla-com-mcp-api-openapi.yml
- filename: neblla-com-stripe-api-openapi.yml
  format: yaml
  label: Neblla Stripe API
  slug: neblla-com-stripe-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/neblla-com/openapi/neblla-com-stripe-api-openapi.yml
auth_types: []
description: Neblla uses OAuth2 token issuance and Bearer token authentication for its MCP API.
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Neblla Authentication
name_suffix: Authentication
oauth_flows: []
overview: Neblla declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: Neblla
provider_slug: neblla-com
scheme_count: 1
schemes:
- evidence: 'Use it as the Bearer token of the MCP server: `https://developers.neblla.com/mcp`.'
  flows:
  - custom_claim
  header: Authorization
  how_to_obtain: POST to the token endpoint with `grant_type=urn:workos:agent-auth:grant-type:claim&claim_token=clm_…` (or refresh with `grant_type=refresh_token&client_id=neblla-agent-auth`).
  location: header
  name: Bearer
  scopes:
  - mcp
  token_url: https://developers.neblla.com/oauth/token
  type: http-bearer
slug: neblla-com-authentication
source_filename: neblla-com-authentication.yml
source_heading: Authentication Profile
source_url: https://neblla.com/auth.md
source_yaml: "generated: '2026-11-19'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://neblla.com/auth.md\nsources:\n- https://neblla.com/auth.md\ndescription: Neblla uses OAuth2 token issuance and Bearer token authentication for its MCP API.\nschemes:\n- type: http-bearer\n  name: Bearer\n  evidence: 'Use it as the Bearer token of the MCP server: `https://developers.neblla.com/mcp`.'\n  location: header\n  header: Authorization\n  flows:\n  - custom_claim\n  token_url: https://developers.neblla.com/oauth/token\n  scopes:\n  - mcp\n  how_to_obtain: POST to the token endpoint with `grant_type=urn:workos:agent-auth:grant-type:claim&claim_token=clm_…` (or refresh with `grant_type=refresh_token&client_id=neblla-agent-auth`).\ndocs: https://neblla.com/auth.md\n"
source_yaml_url: https://artifacts.apis.io/neblla-com/authentication/neblla-com-authentication.yml
summary_line: 1 scheme
tags:
- Company
- Backend
- BaaS
- Gaming
- Artificial Intelligence
- Real-Time
---
