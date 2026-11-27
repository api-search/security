---
anonymous_access: false
api_key_in: []
auth_types: []
description: ''
kind: authentication
layout: security
mechanism_count: 2
method: probed
name: Cocuyo Authentication
name_suffix: Authentication
oauth_flows: []
overview: Cocuyo declares 2 security scheme(s) across its OpenAPI definitions.
provider_name: Cocuyo
provider_slug: cocuyo-ai
scheme_count: 2
schemes:
- authorizationUrl: https://cocuyo.ai/oauth/autorizar
  bearer_methods:
  - header
  evidence: Read from /.well-known/oauth-authorization-server (HTTP 200) and /.well-known/oauth-protected-resource (HTTP 200). OAuth endpoints themselves were not called.
  flow: authorizationCode
  grant_types:
  - authorization_code
  - refresh_token
  issuer: https://cocuyo.ai
  name: oauth2
  pkce: S256
  registrationUrl: https://cocuyo.ai/oauth/registrar
  resource: https://cocuyo.ai/mcp
  revocationUrl: https://cocuyo.ai/oauth/revocar
  scopes:
  - cocuyo:leer
  - cocuyo:crear
  tokenUrl: https://cocuyo.ai/oauth/token
  token_endpoint_auth_methods:
  - none
  type: oauth2
- description: Manual key created under the advanced manual-key option ("Opciones avanzadas — clave manual") on Mis conexiones (web) or Perfil → Conectores (mobile app), used as COCUYO_TOKEN in a terminal. Read-only by default; creation permission and a daily credit limit are set per key. Shown only once.
  evidence: https://cocuyo.ai/conectores.html
  name: connection-key
  scheme: bearer
  type: http
slug: cocuyo-ai-authentication
source_filename: cocuyo-ai-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-04'\nmethod: probed\nsource: https://cocuyo.ai/.well-known/oauth-authorization-server\ndocs: https://cocuyo.ai/conectores.html\nschemes:\n- name: oauth2\n  type: oauth2\n  flow: authorizationCode\n  pkce: S256\n  issuer: https://cocuyo.ai\n  authorizationUrl: https://cocuyo.ai/oauth/autorizar\n  tokenUrl: https://cocuyo.ai/oauth/token\n  registrationUrl: https://cocuyo.ai/oauth/registrar\n  revocationUrl: https://cocuyo.ai/oauth/revocar\n  grant_types: [authorization_code, refresh_token]\n  token_endpoint_auth_methods: [none]\n  scopes: [cocuyo:leer, cocuyo:crear]\n  bearer_methods: [header]\n  resource: https://cocuyo.ai/mcp\n  evidence: Read from /.well-known/oauth-authorization-server (HTTP 200) and /.well-known/oauth-protected-resource (HTTP 200). OAuth endpoints themselves were not called.\n- name: connection-key\n  type: http\n  scheme: bearer\n  description: Manual key created under the advanced manual-key option (\"Opciones avanzadas — clave manual\"\
  ) on Mis conexiones (web) or Perfil → Conectores (mobile app), used as COCUYO_TOKEN in a terminal. Read-only by default; creation permission and a daily credit limit are set per key. Shown only once.\n  evidence: https://cocuyo.ai/conectores.html\n"
source_yaml_url: https://artifacts.apis.io/cocuyo-ai/authentication/cocuyo-ai-authentication.yml
summary_line: 2 schemes
tags:
- Company
- Artificial Intelligence
- Generative AI
- Image Generation
- Video Generation
- Text-to-Speech
- MCP
- Creative Tools
---
