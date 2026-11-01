---
anonymous_access: false
api_key_in: []
api_specs:
- filename: bubblio-dev-agent-keys-api-openapi.yml
  format: yaml
  label: bubblio-dev Agent Keys API
  slug: bubblio-dev-agent-keys-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/bubblio-dev/openapi/bubblio-dev-agent-keys-api-openapi.yml
- filename: bubblio-dev-approvals-api-openapi.yml
  format: yaml
  label: bubblio-dev Approvals API
  slug: bubblio-dev-approvals-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/bubblio-dev/openapi/bubblio-dev-approvals-api-openapi.yml
- filename: bubblio-dev-discovery-api-openapi.yml
  format: yaml
  label: bubblio-dev Discovery API
  slug: bubblio-dev-discovery-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/bubblio-dev/openapi/bubblio-dev-discovery-api-openapi.yml
- filename: bubblio-dev-mcp-api-openapi.yml
  format: yaml
  label: bubblio-dev MCP API
  slug: bubblio-dev-mcp-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/bubblio-dev/openapi/bubblio-dev-mcp-api-openapi.yml
- filename: bubblio-dev-platform-push-api-openapi.yml
  format: yaml
  label: bubblio-dev Platform Push API
  slug: bubblio-dev-platform-push-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/bubblio-dev/openapi/bubblio-dev-platform-push-api-openapi.yml
- filename: bubblio-dev-platform-sync-api-openapi.yml
  format: yaml
  label: bubblio-dev Platform Sync API
  slug: bubblio-dev-platform-sync-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/bubblio-dev/openapi/bubblio-dev-platform-sync-api-openapi.yml
auth_types: []
description: ''
kind: authentication
layout: security
mechanism_count: 2
method: searched
name: Bubblio Dev Authentication
name_suffix: Authentication
oauth_flows: []
overview: bubblio-dev declares 3 security scheme(s) across its OpenAPI definitions.
provider_name: bubblio-dev
provider_slug: bubblio-dev
scheme_count: 3
schemes:
- description: Platform-provided API key for agent operations.
  in: header
  name: bbl_key
  type: apiKey
- bearerFormat: JWT
  description: Consent token JWT from POST /approvals/session.
  scheme: bearer
  type: http
- description: Signed push using X-Bubblio-Signature-V2 and X-Bubblio-Timestamp headers (HMAC-SHA256).
  scheme: custom
  type: http
slug: bubblio-dev-authentication
source_filename: bubblio-dev-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-10-29'\nmethod: searched\nsource: https://bubblio.dev/docs/api\nschemes:\n  - type: apiKey\n    name: bbl_key\n    in: header\n    description: Platform-provided API key for agent operations.\n  - type: http\n    scheme: bearer\n    bearerFormat: JWT\n    description: Consent token JWT from POST /approvals/session.\n  - type: http\n    scheme: custom\n    description: Signed push using X-Bubblio-Signature-V2 and X-Bubblio-Timestamp headers (HMAC-SHA256).\n"
source_yaml_url: https://artifacts.apis.io/bubblio-dev/authentication/bubblio-dev-authentication.yml
summary_line: 3 schemes
tags:
- AI
- Payments
- Automation
- Platform
- Agents
---
