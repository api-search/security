---
api_key_in: []
api_specs:
- filename: end-game-openapi.json
  format: json
  label: Endgame Public API
  slug: endgame-public-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/end-game/refs/heads/main/openapi/end-game-openapi.json
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: End Game Authentication
name_suffix: Authentication
oauth_flows: []
overview: Endgame secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Endgame
provider_slug: end-game
scheme_count: 1
schemes:
- description: 'One of: an Endgame API key prefixed `eak_` (created from Settings → API Keys with a Personal or Org-wide scope), or a WorkOS access token from an Endgame-provisioned M2M application (created from Settings → Applications and exchanged via the `client_credentials` grant).'
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/end-game-openapi.json
  type: http
slug: end-game-authentication
source_filename: end-game-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: derived\nsource: openapi/end-game-openapi.json\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  description: 'One of: an Endgame API key prefixed `eak_` (created from Settings → API Keys\n    with a Personal or Org-wide scope), or a WorkOS access token from an Endgame-provisioned\n    M2M application (created from Settings → Applications and exchanged via the `client_credentials`\n    grant).'\n  sources:\n  - openapi/end-game-openapi.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/end-game/refs/heads/main/authentication/end-game-authentication.yml
summary_line: http · 1 scheme
tags:
- Company
- Sales
- Revenue Intelligence
- Go-To-Market
- Artificial Intelligence
- Agents
- MCP
- Knowledge Graph
- CRM
- Conversation Intelligence
---
