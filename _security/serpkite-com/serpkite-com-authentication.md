---
anonymous_access: false
api_key_in: []
api_specs:
- filename: serpkite-com-openapi-generated.yml
  format: yaml
  label: serpkite-com API
  slug: serpkite-com-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/serpkite-com/openapi/_ae-authored/serpkite-com-openapi-generated.yml
auth_types: []
description: Authentication methods for SerpKite API
kind: authentication
layout: security
mechanism_count: 2
method: searched
name: Serpkite Com Authentication
name_suffix: Authentication
oauth_flows: []
overview: serpkite-com declares 2 security scheme(s) across its OpenAPI definitions.
provider_name: serpkite-com
provider_slug: serpkite-com
scheme_count: 2
schemes:
- evidence: Send the key as a Bearer token in the `Authorization` header.
  header: Authorization
  location: header
  name: API key (Bearer header)
  type: apiKey
- evidence: 'OAuth access token `Authorization: Bearer skt_oat_…` the MCP server only, issued when you approve an MCP client.'
  header: Authorization
  location: header
  name: OAuth access token (MCP server)
  type: apiKey
slug: serpkite-com-authentication
source_filename: serpkite-com-authentication.yml
source_heading: Authentication Profile
source_url: https://serpkite.com/docs/authentication.md
source_yaml: "generated: '2026-10-31'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://serpkite.com/docs/authentication.md\nsources:\n- https://serpkite.com/docs/authentication.md\n- https://serpkite.com/docs/api-keys.md\n- https://serpkite.com/docs/authentication\n- https://serpkite.com/docs/api-keys\ndescription: Authentication methods for SerpKite API\nschemes:\n- type: apiKey\n  name: API key (Bearer header)\n  evidence: Send the key as a Bearer token in the `Authorization` header.\n  location: header\n  header: Authorization\n- type: apiKey\n  name: OAuth access token (MCP server)\n  evidence: 'OAuth access token `Authorization: Bearer skt_oat_…` the MCP server only, issued when you approve an MCP client.'\n  location: header\n  header: Authorization\nnote: No OAuth2 flows, HTTP basic, JWT, HMAC, or MTLS are documented. 3 extracted row(s) were dropped because their quote was not on the page.\ndocs: https://serpkite.com/docs/authentication.md\n"
source_yaml_url: https://artifacts.apis.io/serpkite-com/authentication/serpkite-com-authentication.yml
summary_line: 2 schemes
tags:
- Company
- Search
- Data Retrieval
- API
- Developer Platform
---
