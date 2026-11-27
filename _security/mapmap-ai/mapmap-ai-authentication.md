---
anonymous_access: false
api_key_in: []
api_specs:
- filename: mapmap-ai-openapi-generated.yml
  format: yaml
  label: MapMap AI API
  slug: mapmap-ai-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/mapmap-ai/openapi/_ae-authored/mapmap-ai-openapi-generated.yml
auth_types: []
description: Authentication schemes as published on MapMap AI docs
kind: authentication
layout: security
mechanism_count: 3
method: searched
name: MapMap AI Authentication
name_suffix: Authentication
oauth_flows: []
overview: MapMap AI declares 3 security scheme(s) across its OpenAPI definitions.
provider_name: MapMap AI
provider_slug: mapmap-ai
scheme_count: 3
schemes:
- evidence: 'Copy Authorization: Bearer snk_... # preferred'
  header: Authorization
  location: header
  name: Bearer
  type: http-bearer
- evidence: '? api_key =snk_... # query parameter, for clients that cannot set headers (e.g. tile URLs)'
  location: query
  name: api_key
  type: apiKey
- evidence: 'OAuth for agent clients: GET /.well-known/oauth-authorization-server , POST /oauth/register and POST /oauth/token'
  flows:
  - GET /.well-known/oauth-authorization-server
  - POST /oauth/token
  name: OAuth
  type: oauth2
slug: mapmap-ai-authentication
source_filename: mapmap-ai-authentication.yml
source_heading: Authentication Profile
source_url: https://mapmap.ai/docs/conventions
source_yaml: "generated: '2026-11-17'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://mapmap.ai/docs/conventions\nsources:\n- https://mapmap.ai/docs/conventions\n- https://mapmap.ai/docs/mapbox-compatible-api\n- https://mapmap.ai/docs/quickstart\n- https://mapmap.ai/docs/quickstart.md\ndescription: Authentication schemes as published on MapMap AI docs\nschemes:\n- type: http-bearer\n  name: Bearer\n  evidence: 'Copy Authorization: Bearer snk_... # preferred'\n  location: header\n  header: Authorization\n- type: apiKey\n  name: api_key\n  evidence: '? api_key =snk_... # query parameter, for clients that cannot set headers (e.g. tile URLs)'\n  location: query\n- type: oauth2\n  name: OAuth\n  evidence: 'OAuth for agent clients: GET /.well-known/oauth-authorization-server , POST /oauth/register and POST /oauth/token'\n  flows:\n  - GET /.well-known/oauth-authorization-server\n  - POST /oauth/token\ndocs: https://mapmap.ai/docs/conventions\n"
source_yaml_url: https://artifacts.apis.io/mapmap-ai/authentication/mapmap-ai-authentication.yml
summary_line: 3 schemes
tags:
- Company
- Navigation
- Artificial Intelligence
- Mapping
- Fleet Management
---
