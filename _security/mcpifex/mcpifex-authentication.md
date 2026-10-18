---
anonymous_access: false
api_key_in: []
api_specs:
- filename: mcpifex-openapi-generated.yml
  format: yaml
  label: Amdose API
  slug: mcpifex-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mcpifex/refs/heads/main/openapi/_ae-authored/mcpifex-openapi-generated.yml
auth_types: []
description: Authentication for the MCPifex gateway uses an API key that starts with "mcpx_".
kind: authentication
layout: security
mechanism_count: 2
method: searched
name: Mcpifex Authentication
name_suffix: Authentication
oauth_flows: []
overview: Amdose declares 2 security scheme(s) across its OpenAPI definitions.
provider_name: Amdose
provider_slug: mcpifex
scheme_count: 2
schemes:
- evidence: 'You send it in an Authorization: Bearer header, or as the first segment of the URL if your client can''t set headers.'
  header: Authorization
  how_to_obtain: Create an instance in the portal, choose enabled tools, and generate the key on the API key page. The key is shown once.
  location: header
  name: Authorization
  type: http-bearer
- evidence: 'You send it in an Authorization: Bearer header, or as the first segment of the URL if your client can''t set headers.'
  how_to_obtain: Create an instance in the portal, choose enabled tools, and generate the key on the API key page. The key is shown once.
  location: path
  name: Path segment
  type: apiKey
slug: mcpifex-authentication
source_filename: mcpifex-authentication.yml
source_heading: Authentication Profile
source_url: https://mcpifex.com/docs/api-keys-and-authentication
source_yaml: "generated: '2026-10-18'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://mcpifex.com/docs/api-keys-and-authentication\nsources:\n- https://mcpifex.com/docs/api-keys-and-authentication\n- https://mcpifex.com/docs/api-keys-and-authentication.md\n- https://mcpifex.com/docs/connected-accounts-oauth\n- https://mcpifex.com/docs/connected-accounts-oauth.md\ndescription: Authentication for the MCPifex gateway uses an API key that starts with \"mcpx_\".\nschemes:\n- type: http-bearer\n  name: Authorization\n  evidence: 'You send it in an Authorization: Bearer header, or as the first segment of the URL if your client can''t set headers.'\n  location: header\n  header: Authorization\n  how_to_obtain: Create an instance in the portal, choose enabled tools, and generate the key on the API key page. The key is shown once.\n- type: apiKey\n  name: Path segment\n  evidence: 'You send it in an Authorization: Bearer header, or as the first segment of the URL if\
  \ your client can''t set headers.'\n  location: path\n  how_to_obtain: Create an instance in the portal, choose enabled tools, and generate the key on the API key page. The key is shown once.\nnote: No OAuth2 flows, client credentials, or other authentication types are described on the provided pages.\ndocs: https://mcpifex.com/docs/api-keys-and-authentication\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/mcpifex/refs/heads/main/authentication/mcpifex-authentication.yml
summary_line: 2 schemes
tags:
- Company
- MCP
- Marketplace
- AI-Agents
- Integration
---
