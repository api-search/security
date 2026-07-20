---
api_key_in: []
auth_types:
- oauth2
description: ''
kind: authentication
layout: security
method: searched
name: Lightsprint Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: Lightsprint secures its APIs with oauth2 across 1 declared security scheme, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: Lightsprint
provider_slug: lightsprint
scheme_count: 1
schemes:
- display_name: Lightsprint OAuth2 API
  flows:
  - authorizationUrl: https://lightsprint.ai/oauth/authorize
    flow: authorizationCode
    scope_count: 7
    scopes_artifact: scopes/lightsprint-scopes.yml
    tokenUrl: https://lightsprint.ai/oauth/token
  name: LightsprintOAuth2Api
  sources:
  - https://github.com/SprintsAI/n8n-nodes-lightsprint/blob/main/credentials/LightsprintOAuth2Api.credentials.ts
  type: oauth2
slug: lightsprint-authentication
source_filename: lightsprint-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: searched\nsource: https://github.com/SprintsAI/n8n-nodes-lightsprint/blob/main/credentials/LightsprintOAuth2Api.credentials.ts\nnotes: >-\n  Lightsprint publishes no OpenAPI document, so this profile was NOT derived from a\n  spec. It is captured from the provider's own published OAuth 2.0 credential\n  definition in the first-party n8n community node, corroborated by the on-demand\n  browser OAuth flow described in the Claude Code plugin README. Values are recorded\n  verbatim from those sources.\ndocs: https://github.com/SprintsAI/n8n-nodes-lightsprint\nsummary:\n  types: [oauth2]\n  api_key_in: []\n  oauth2_flows: [authorizationCode]\n  token_placement: header\n  token_refresh: automatic (CLI refreshes saved tokens)\nschemes:\n- name: LightsprintOAuth2Api\n  type: oauth2\n  display_name: Lightsprint OAuth2 API\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://lightsprint.ai/oauth/authorize\n    tokenUrl: https://lightsprint.ai/oauth/token\n\
  \    scope_count: 7\n    scopes_artifact: scopes/lightsprint-scopes.yml\n  sources:\n  - https://github.com/SprintsAI/n8n-nodes-lightsprint/blob/main/credentials/LightsprintOAuth2Api.credentials.ts\nverification:\n  endpoint: GET /api/repo-key/info\n  base_url: https://lightsprint.ai\n  purpose: credential test — resolves the caller's repo/workspace id from the access\n    token\ntenancy:\n  unit: workspace\n  note: >-\n    An access token is bound to one Lightsprint workspace; the repo id is resolved\n    from the token via /api/repo-key/info rather than being passed by the client.\ngaps:\n- No public, human-readable authentication documentation page was found on\n  lightsprint.ai — the auth contract is only discoverable from the published client\n  source. No API-key alternative, no OIDC discovery document, no mutualTLS.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/lightsprint/refs/heads/main/authentication/lightsprint-authentication.yml
summary_line: oauth2 · 1 scheme
tags:
- Company
- Developer Tools
- Artificial Intelligence
- Agents
- Software Development
- Project Management
- Code Generation
- Team Collaboration
---
