---
anonymous_access: false
api_key_in: []
api_specs:
- filename: cleolm-com-tools-api-openapi.yml
  format: yaml
  label: CleoLM Tools API
  slug: cleolm-com-tools-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/cleolm-com/openapi/cleolm-com-tools-api-openapi.yml
auth_types:
- http
- oauth2
description: ''
kind: authentication
layout: security
mechanism_count: 2
method: searched
name: CleoLM Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: CleoLM secures its APIs with http and oauth2 across 2 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: CleoLM
provider_slug: cleolm-com
scheme_count: 2
schemes:
- description: A CleoLM API key (clm_live_…) from https://cleolm.com/developers, or an OAuth access token.
  name: bearer
  scheme: bearer
  sources:
  - openapi/cleolm-com-openapi.yml
  type: http
- flows:
  - authorizationUrl: https://cleolm.com/oauth/authorize
    flow: authorizationCode
    scopes: 2
    tokenUrl: https://cleolm.com/oauth/token
  name: oauth2
  sources:
  - openapi/cleolm-com-openapi.yml
  type: oauth2
slug: cleolm-com-authentication
source_filename: cleolm-com-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-04'\nmethod: searched\nsource: https://cleolm.com/llms.txt\nsummary:\n  types:\n  - http\n  - oauth2\n  oauth2_flows:\n  - authorizationCode\nschemes:\n- name: bearer\n  type: http\n  scheme: bearer\n  description: A CleoLM API key (clm_live_…) from https://cleolm.com/developers, or\n    an OAuth access token.\n  sources:\n  - openapi/cleolm-com-openapi.yml\n- name: oauth2\n  type: oauth2\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://cleolm.com/oauth/authorize\n    tokenUrl: https://cleolm.com/oauth/token\n    scopes: 2\n  sources:\n  - openapi/cleolm-com-openapi.yml\ndocs: https://cleolm.com/developers\nderived_from: openapi/cleolm-com-openapi.yml\nnotes:\n- OAuth 2.1 with PKCE S256, Dynamic Client Registration and Client ID Metadata Documents.\n  Clients that support it only need the MCP URL.\n- 'Or an API key: Authorization: Bearer clm_live_... Users create and revoke keys\n  at https://cleolm.com/developers. Keys are shown once,\
  \ can be scoped to exclude\n  ingest, and stop working within 60 seconds of revocation.'\n- 'OAuth protected-resource metadata: https://cleolm.com/.well-known/oauth-protected-resource/mcp\n  ; authorization-server metadata: https://cleolm.com/.well-known/oauth-authorization-server\n  (documented in llms.txt; not called by this pass).'\n- No-auth endpoint https://cleolm.com/mcp/open exposes search, get_passage and list_channels\n  only.\nkey_prefixes:\n- prefix: clm_live_\n  mode: live\n"
source_yaml_url: https://artifacts.apis.io/cleolm-com/authentication/cleolm-com-authentication.yml
summary_line: http/oauth2 · 2 schemes
tags:
- Company
- Artificial Intelligence
- Transcription
- Podcasts
- YouTube
- Search
- MCP
- Video
---
