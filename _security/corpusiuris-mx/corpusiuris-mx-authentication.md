---
anonymous_access: true
api_key_in: []
api_specs:
- filename: corpusiuris-mx-agent-api-openapi.yml
  format: yaml
  label: Corpus Iuris Agent API
  slug: corpusiuris-mx-agent-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/corpusiuris-mx/openapi/corpusiuris-mx-agent-api-openapi.yml
auth_types:
- none
- http
- oauth2
description: ''
kind: authentication
layout: security
mechanism_count: 3
method: searched
name: Corpus Iuris Authentication
name_suffix: Authentication
oauth_flows: []
overview: Corpus Iuris secures its APIs with none, http, and oauth2 across 4 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Corpus Iuris
provider_slug: corpusiuris-mx
scheme_count: 4
schemes:
- applies_to: https://corpusiuris.mx/api/agent/v1/*
  description: 'REST agent API works without a key: ''Sin API key. Sin registro.'' Anonymous lane is metered per IP.'
  name: Anonymous
  sources:
  - https://corpusiuris.mx/agentes
  type: none
- description: Token personal `ci_agent_…` (Mi cuenta → Conecta tu IA). Sin él se usa el carril anónimo; con uno inválido se devuelve 401.
  name: TokenPersonal
  scheme: bearer
  sources:
  - openapi/corpusiuris-mx-openapi.yml
  token_prefix: ci_agent_
  type: http
- description: 'Partner lane (carril E) for ATERAsoft allied platforms (today LegalAdmin): key ci_partner_… verified by key, not IP; X-Partner-Tenant header counts and attributes but does not authorize. Keys issued in the Corpus Iuris panel. Exact header not documented.'
  name: PartnerKey
  sources:
  - https://corpusiuris.mx/agentes
  token_prefix: ci_partner_
  type: apiKey
- applies_to: https://api.corpusiuris.mx/mcp
  description: OAuth 2.0 with dynamic client registration (RFC 7591) and PKCE S256 for the remote MCP connector.
  flows:
    authorizationCode:
      code_challenge_methods:
      - S256
      grant_types:
      - authorization_code
      - refresh_token
      metadata: https://api.corpusiuris.mx/.well-known/oauth-authorization-server
      scopes:
      - search
      - perfil
  name: McpOAuth
  sources:
  - https://corpusiuris.mx/agentes
  - https://api.corpusiuris.mx/.well-known/oauth-authorization-server
  type: oauth2
slug: corpusiuris-mx-authentication
source_filename: corpusiuris-mx-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-04'\nmethod: searched\nsource: https://corpusiuris.mx/agentes\ndocs: https://corpusiuris.mx/agentes\nsummary:\n  types:\n  - none\n  - http\n  - oauth2\nschemes:\n- name: Anonymous\n  type: none\n  description: \"REST agent API works without a key: 'Sin API key. Sin registro.' Anonymous lane is metered per IP.\"\n  applies_to: https://corpusiuris.mx/api/agent/v1/*\n  sources:\n  - https://corpusiuris.mx/agentes\n- name: TokenPersonal\n  type: http\n  scheme: bearer\n  token_prefix: ci_agent_\n  description: Token personal `ci_agent_…` (Mi cuenta → Conecta tu IA). Sin él se usa el carril\n    anónimo; con uno inválido se devuelve 401.\n  sources:\n  - openapi/corpusiuris-mx-openapi.yml\n- name: PartnerKey\n  type: apiKey\n  token_prefix: ci_partner_\n  description: \"Partner lane (carril E) for ATERAsoft allied platforms (today LegalAdmin): key ci_partner_… verified by key, not IP; X-Partner-Tenant header counts and attributes but does not authorize. Keys\
  \ issued in the Corpus Iuris panel. Exact header not documented.\"\n  sources:\n  - https://corpusiuris.mx/agentes\n- name: McpOAuth\n  type: oauth2\n  applies_to: https://api.corpusiuris.mx/mcp\n  description: OAuth 2.0 with dynamic client registration (RFC 7591) and PKCE S256 for the remote MCP connector.\n  flows:\n    authorizationCode:\n      metadata: https://api.corpusiuris.mx/.well-known/oauth-authorization-server\n      grant_types: [authorization_code, refresh_token]\n      code_challenge_methods: [S256]\n      scopes: [search, perfil]\n  sources:\n  - https://corpusiuris.mx/agentes\n  - https://api.corpusiuris.mx/.well-known/oauth-authorization-server\n"
source_yaml_url: https://artifacts.apis.io/corpusiuris-mx/authentication/corpusiuris-mx-authentication.yml
summary_line: none/http/oauth2 · 4 schemes
tags:
- Company
- Legal
- Legal Research
- Artificial Intelligence
- Mexico
- Jurisprudence
- MCP
- Search
---
