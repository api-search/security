---
anonymous_access: false
api_key_in: []
api_specs:
- filename: findlocal-events-api-openapi.yml
  format: yaml
  label: FindLocal Events API
  slug: findlocal-events-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/findlocal/openapi/findlocal-events-api-openapi.yml
- filename: findlocal-venues-api-openapi.yml
  format: yaml
  label: FindLocal Venues API
  slug: findlocal-venues-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/findlocal/openapi/findlocal-venues-api-openapi.yml
auth_types: []
description: ''
kind: authentication
layout: security
mechanism_count: 2
method: searched
name: FindLocal Authentication
name_suffix: Authentication
oauth_flows: []
overview: FindLocal declares 2 security scheme(s) across its OpenAPI definitions.
provider_name: FindLocal
provider_slug: findlocal
scheme_count: 2
schemes:
- alternate_header: X-API-Key
  applies_to: REST API (/api/events, /api/events/{id}, /api/venues)
  evidence: 'Every /api/events, /api/events/{id} and /api/venues call needs a key: Authorization: Bearer <key> (or X-API-Key: <key>).'
  header: Authorization
  how_to_obtain: Create a free account at https://findlocal.community/signup (no card) and mint a key at https://findlocal.community/dashboard/keys. One account can hold 5 named keys.
  name: Bearer API key
  scheme: bearer
  type: http
- applies_to: MCP server (https://mcp.findlocal.community/mcp)
  evidence: 'MCP server endpoint: https://mcp.findlocal.community/mcp (Streamable HTTP; OAuth 2.1 + PKCE). On first connect you paste an API key.'
  flows:
  - authorization_code
  how_to_obtain: The same account API key authorises the MCP server; you paste it on first connect through the OAuth consent flow.
  name: OAuth 2.1 with PKCE
  type: oauth2
slug: findlocal-authentication
source_filename: findlocal-authentication.yml
source_heading: Authentication Profile
source_url: https://findlocal.community/llms-full.txt
source_yaml: "generated: '2026-11-04'\nmethod: searched\ngenerator: docs module\nsource: https://findlocal.community/llms-full.txt\nsources:\n- https://findlocal.community/llms-full.txt\n- https://findlocal.community/openapi.json\nschemes:\n- type: http\n  name: Bearer API key\n  scheme: bearer\n  evidence: 'Every /api/events, /api/events/{id} and /api/venues call needs a key: Authorization: Bearer <key> (or X-API-Key: <key>).'\n  how_to_obtain: Create a free account at https://findlocal.community/signup (no card) and mint a key at https://findlocal.community/dashboard/keys. One account can hold 5 named keys.\n  header: Authorization\n  alternate_header: X-API-Key\n  applies_to: REST API (/api/events, /api/events/{id}, /api/venues)\n- type: oauth2\n  name: OAuth 2.1 with PKCE\n  evidence: 'MCP server endpoint: https://mcp.findlocal.community/mcp (Streamable HTTP; OAuth 2.1 + PKCE). On first connect you paste an API key.'\n  flows:\n  - authorization_code\n  applies_to: MCP server (https://mcp.findlocal.community/mcp)\n\
  \  how_to_obtain: The same account API key authorises the MCP server; you paste it on first connect through the OAuth consent flow.\ndocs: https://findlocal.community/docs\nnotes: One account key authorises both the REST API and the MCP server. Playground server (/api/playground) needs no key.\n"
source_yaml_url: https://artifacts.apis.io/findlocal/authentication/findlocal-authentication.yml
summary_line: 2 schemes
tags:
- Event
- Hyperlocal
- Community
- Data
- Open Data
---
