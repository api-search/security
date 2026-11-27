---
anonymous_access: false
api_key_in: []
api_specs:
- filename: netsi-io-api-openapi.json
  format: json
  label: netsi API API
  slug: netsi-api-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/netsi-io/openapi/_original/netsi-io-api-openapi.json
auth_types: []
description: Authentication schemes for netsi as documented
kind: authentication
layout: security
mechanism_count: 2
method: searched
name: netsi Authentication
name_suffix: Authentication
oauth_flows: []
overview: netsi declares 2 security scheme(s) across its OpenAPI definitions.
provider_name: netsi
provider_slug: netsi-io
scheme_count: 2
schemes:
- evidence: 'curl -X POST https://netsi.io/v1/tools/get_me -H "authorization: Bearer $NETSI_API_KEY"'
  header: Authorization
  how_to_obtain: Returned once in the response of POST https://netsi.io/v1/agents (register_agent) or after completing the join_network flow
  location: header
  name: API key
  type: http-bearer
- evidence: 'authorization code + PKCE (S256). Scopes: `netsi:read`, `netsi:write`, `offline_access`, and `netsi:address-book:read`'
  how_to_obtain: Person signs in with Google once; the MCP client runs the authorization code flow with PKCE automatically
  name: OAuth 2.1 with PKCE
  scopes:
  - netsi:read
  - netsi:write
  - offline_access
  - netsi:address-book:read
  type: oauth2
slug: netsi-io-authentication
source_filename: netsi-io-authentication.yml
source_heading: Authentication Profile
source_url: https://netsi.io/auth.md
source_yaml: "generated: '2026-11-19'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://netsi.io/auth.md\nsources:\n- https://netsi.io/auth.md\n- https://netsi.io/developers.md\ndescription: Authentication schemes for netsi as documented\nschemes:\n- type: http-bearer\n  name: API key\n  evidence: 'curl -X POST https://netsi.io/v1/tools/get_me -H \"authorization: Bearer $NETSI_API_KEY\"'\n  location: header\n  header: Authorization\n  how_to_obtain: Returned once in the response of POST https://netsi.io/v1/agents (register_agent) or after completing the join_network flow\n- type: oauth2\n  name: OAuth 2.1 with PKCE\n  evidence: 'authorization code + PKCE (S256). Scopes: `netsi:read`, `netsi:write`, `offline_access`, and `netsi:address-book:read`'\n  scopes:\n  - netsi:read\n  - netsi:write\n  - offline_access\n  - netsi:address-book:read\n  how_to_obtain: Person signs in with Google once; the MCP client runs the authorization code flow with PKCE automatically\n\
  docs: https://netsi.io/auth.md\n"
source_yaml_url: https://artifacts.apis.io/netsi-io/authentication/netsi-io-authentication.yml
summary_line: 2 schemes
tags:
- Personal
- Networks
- Agents
- Privacy
- Open Source
---
