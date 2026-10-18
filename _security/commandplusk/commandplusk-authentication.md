---
anonymous_access: false
api_key_in: []
api_specs:
- filename: commandplusk-cmdk-api-openapi.yml
  format: yaml
  label: CMD+K Cmdk API
  slug: commandplusk-cmdk-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/commandplusk/refs/heads/main/openapi/commandplusk-cmdk-api-openapi.yml
- filename: commandplusk-models-api-openapi.yml
  format: yaml
  label: CMD+K Models API
  slug: commandplusk-models-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/commandplusk/refs/heads/main/openapi/commandplusk-models-api-openapi.yml
- filename: commandplusk-public-api-openapi.yml
  format: yaml
  label: CMD+K Public API
  slug: commandplusk-public-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/commandplusk/refs/heads/main/openapi/commandplusk-public-api-openapi.yml
auth_types: []
description: Authentication modes for CMD+K MCP deployments as described in the documentation.
kind: authentication
layout: security
mechanism_count: 3
method: searched
name: Commandplusk Authentication
name_suffix: Authentication
oauth_flows: []
overview: CMD+K declares 3 security scheme(s) across its OpenAPI definitions.
provider_name: CMD+K
provider_slug: commandplusk
scheme_count: 3
schemes:
- evidence: Customers use their own API keys (recommended). Each customer opens your MCP's connect page and pastes the API key they already have with your product.
  how_to_obtain: Customer provides the existing API key from your product on the MCP connect page.
  name: Per‑customer API key
  type: apiKey
- evidence: Customers sign in with your OAuth. Same per‑customer identity, via your OAuth server. Configure your authorize/token URLs and client ID in the Privacy tab; we run the full authorization‑code flow (with PKCE) and refresh tokens automatically.
  flows:
  - authorization_code
  how_to_obtain: Configure authorize and token URLs and client ID in the CMD+K deployment's Privacy tab; CMD+K runs the PKCE‑enabled authorization‑code flow.
  name: Per‑customer OAuth
  type: oauth2
- evidence: Shared access token (internal/team edge case). All callers use the workspace's stored token — your API cannot tell them apart.
  header: Authorization
  how_to_obtain: Workspace stores a token that is used for all calls; no per‑customer credential is required.
  location: header
  name: Shared access token (internal/team edge case)
  type: http-bearer
slug: commandplusk-authentication
source_filename: commandplusk-authentication.yml
source_heading: Authentication Profile
source_url: https://commandplusk.com/docs/build-mcp/authentication
source_yaml: "generated: '2026-10-16'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://commandplusk.com/docs/build-mcp/authentication\nsources:\n- https://commandplusk.com/docs/build-mcp/authentication\n- https://commandplusk.com/docs/widget/end-user-oauth\n- https://commandplusk.com/docs/widget/jwt-auth\n- https://commandplusk.com/docs/widget/overview\ndescription: Authentication modes for CMD+K MCP deployments as described in the documentation.\nschemes:\n- type: apiKey\n  name: Per‑customer API key\n  evidence: Customers use their own API keys (recommended). Each customer opens your MCP's connect page and pastes the API key they already have\n    with your product.\n  how_to_obtain: Customer provides the existing API key from your product on the MCP connect page.\n- type: oauth2\n  name: Per‑customer OAuth\n  evidence: Customers sign in with your OAuth. Same per‑customer identity, via your OAuth server. Configure your authorize/token URLs and client\n \
  \   ID in the Privacy tab; we run the full authorization‑code flow (with PKCE) and refresh tokens automatically.\n  flows:\n  - authorization_code\n  how_to_obtain: Configure authorize and token URLs and client ID in the CMD+K deployment's Privacy tab; CMD+K runs the PKCE‑enabled authorization‑code\n    flow.\n- type: http-bearer\n  name: Shared access token (internal/team edge case)\n  evidence: Shared access token (internal/team edge case). All callers use the workspace's stored token — your API cannot tell them apart.\n  location: header\n  header: Authorization\n  how_to_obtain: Workspace stores a token that is used for all calls; no per‑customer credential is required.\ndocs: https://commandplusk.com/docs/build-mcp/authentication\nnote: 1 extracted row(s) were dropped because their quote was not on the page.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/commandplusk/refs/heads/main/authentication/commandplusk-authentication.yml
summary_line: 3 schemes
tags:
- Artificial Intelligence
- Assistant
- Platform
- Software-as-a-Service
- Developers
---
