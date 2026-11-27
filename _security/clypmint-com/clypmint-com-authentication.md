---
anonymous_access: false
api_key_in: []
api_specs:
- filename: clypmint-com-assets-api-openapi.yml
  format: yaml
  label: Clypmint Assets API
  slug: clypmint-com-assets-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/clypmint-com/openapi/clypmint-com-assets-api-openapi.yml
- filename: clypmint-com-content-plans-api-openapi.yml
  format: yaml
  label: Clypmint Content Plans API
  slug: clypmint-com-content-plans-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/clypmint-com/openapi/clypmint-com-content-plans-api-openapi.yml
- filename: clypmint-com-me-api-openapi.yml
  format: yaml
  label: Clypmint Me API
  slug: clypmint-com-me-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/clypmint-com/openapi/clypmint-com-me-api-openapi.yml
- filename: clypmint-com-memory-api-openapi.yml
  format: yaml
  label: Clypmint Memory API
  slug: clypmint-com-memory-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/clypmint-com/openapi/clypmint-com-memory-api-openapi.yml
- filename: clypmint-com-openapi-json-api-openapi.yml
  format: yaml
  label: Clypmint Openapi.json API
  slug: clypmint-com-openapi-json-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/clypmint-com/openapi/clypmint-com-openapi-json-api-openapi.yml
- filename: clypmint-com-schedule-api-openapi.yml
  format: yaml
  label: Clypmint Schedule API
  slug: clypmint-com-schedule-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/clypmint-com/openapi/clypmint-com-schedule-api-openapi.yml
- filename: clypmint-com-styles-api-openapi.yml
  format: yaml
  label: Clypmint Styles API
  slug: clypmint-com-styles-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/clypmint-com/openapi/clypmint-com-styles-api-openapi.yml
- filename: clypmint-com-videos-api-openapi.yml
  format: yaml
  label: Clypmint Videos API
  slug: clypmint-com-videos-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/clypmint-com/openapi/clypmint-com-videos-api-openapi.yml
auth_types:
- http
- oauth2
description: ''
kind: authentication
layout: security
mechanism_count: 3
method: searched
name: Clypmint Authentication
name_suffix: Authentication
oauth_flows: []
overview: Clypmint secures its APIs with http and oauth2 across 3 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Clypmint
provider_slug: clypmint-com
scheme_count: 3
schemes:
- bearerFormat: API key or OAuth token
  description: Create a cm_live_... API key in Studio settings. Send it as a bearer token.
  key_prefix: cm_live_
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/clypmint-com-openapi.yml
  - https://clypmint.com/developers
  type: http
- authorization_servers:
  - https://clypmint.com
  description: The MCP server at https://clypmint.com/mcp uses Streamable HTTP and OAuth 2.1 sign-in. Its protected-resource metadata names https://clypmint.com as authorization server.
  name: mcpOAuth
  scopes:
  - clypmint
  - clypmint.publish
  sources:
  - https://clypmint.com/developers
  - https://clypmint.com/.well-known/oauth-protected-resource
  type: oauth2
- applies_to: B-Roll API (https://clypmint.com/api/v1/broll) and https://clypmint.com/mcp/broll
  description: Make a key in the dashboard. It starts with cm_live_ and is shown once. Send it as a bearer token on every request.
  name: brollApiKey
  scheme: bearer
  sources:
  - https://clypmint.com/broll/docs
  type: http
slug: clypmint-com-authentication
source_filename: clypmint-com-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-04'\nmethod: searched\nsource: https://clypmint.com/developers\ndocs: https://clypmint.com/developers\nsummary:\n  types:\n  - http\n  - oauth2\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: API key or OAuth token\n  description: Create a cm_live_... API key in Studio settings. Send it as a bearer token.\n  key_prefix: cm_live_\n  sources:\n  - openapi/clypmint-com-openapi.yml\n  - https://clypmint.com/developers\n- name: mcpOAuth\n  type: oauth2\n  description: The MCP server at https://clypmint.com/mcp uses Streamable HTTP and OAuth 2.1 sign-in. Its protected-resource metadata names https://clypmint.com as authorization server.\n  authorization_servers:\n  - https://clypmint.com\n  scopes:\n  - clypmint\n  - clypmint.publish\n  sources:\n  - https://clypmint.com/developers\n  - https://clypmint.com/.well-known/oauth-protected-resource\n- name: brollApiKey\n  type: http\n  scheme: bearer\n  applies_to: B-Roll API (https://clypmint.com/api/v1/broll)\
  \ and https://clypmint.com/mcp/broll\n  description: Make a key in the dashboard. It starts with cm_live_ and is shown once. Send it as a bearer token on every request.\n  sources:\n  - https://clypmint.com/broll/docs\n"
source_yaml_url: https://artifacts.apis.io/clypmint-com/authentication/clypmint-com-authentication.yml
summary_line: http/oauth2 · 3 schemes
tags:
- Company
- AI Video Editing
- Video
- Generative AI
- Content Creation
- MCP
- Creator Tools
- Short-Form Video
---
