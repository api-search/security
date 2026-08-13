---
api_key_in:
- header
api_specs:
- filename: effect-photonics-wp-v2-api-openapi.yml
  format: yaml
  label: EFFECT Photonics Wp/v2 API
  slug: effect-photonics-wp-v2-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/effect-photonics/refs/heads/main/openapi/effect-photonics-wp-v2-api-openapi.yml
- filename: effect-photonics-effect-v1-api-openapi.yml
  format: yaml
  label: EFFECT Photonics Effect/v1 API
  slug: effect-photonics-effect-v1-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/effect-photonics/refs/heads/main/openapi/effect-photonics-effect-v1-api-openapi.yml
- filename: effect-photonics-mcp-api-openapi.yml
  format: yaml
  label: EFFECT Photonics MCP API
  slug: effect-photonics-mcp-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/effect-photonics/refs/heads/main/openapi/effect-photonics-mcp-api-openapi.yml
- filename: effect-photonics-wp-abilities-v1-api-openapi.yml
  format: yaml
  label: EFFECT Photonics Wp Abilities/v1 API
  slug: effect-photonics-wp-abilities-v1-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/effect-photonics/refs/heads/main/openapi/effect-photonics-wp-abilities-v1-api-openapi.yml
- filename: effect-photonics-oembed-1-0-api-openapi.yml
  format: yaml
  label: EFFECT Photonics Oembed/1.0 API
  slug: effect-photonics-oembed-1-0-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/effect-photonics/refs/heads/main/openapi/effect-photonics-oembed-1-0-api-openapi.yml
- filename: effect-photonics-root-api-openapi.yml
  format: yaml
  label: EFFECT Photonics Root API
  slug: effect-photonics-root-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/effect-photonics/refs/heads/main/openapi/effect-photonics-root-api-openapi.yml
auth_types:
- apiKey
- http
- oauth2
description: ''
kind: authentication
layout: security
method: derived
name: Effect Photonics Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: EFFECT Photonics secures its APIs with apiKey, http, and oauth2 across 3 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: EFFECT Photonics
provider_slug: effect-photonics
scheme_count: 3
schemes:
- description: OAuth 2.1 authorization-code + PKCE (S256), as advertised by the provider's RFC 8414 metadata at https://effectphotonics.com/.well-known/oauth-authorization-server (fetched 2026-08-12, HTTP 200). Guards the `mcp` namespace; the protected-resource metadata (RFC 9728) names https://effectphotonics.com/wp-json/mcp/mcp-oauth-server.
  flows:
  - authorizationUrl: https://effectphotonics.com/oauth/authorize
    flow: authorizationCode
    scopes: 1
    tokenUrl: https://effectphotonics.com/oauth/token
  name: mcpOAuth2
  sources:
  - openapi/effect-photonics-effect-v1-api-openapi.yml
  - openapi/effect-photonics-mcp-api-openapi.yml
  - openapi/effect-photonics-oembed-1-0-api-openapi.yml
  - openapi/effect-photonics-root-api-openapi.yml
  - openapi/effect-photonics-wp-abilities-v1-api-openapi.yml
  - openapi/effect-photonics-wp-v2-api-openapi.yml
  type: oauth2
- description: WordPress cookie-authentication nonce. Advertised by the live server in its Access-Control-Allow-Headers response header (Authorization, X-WP-Nonce, Content-Disposition, Content-MD5, Content-Type).
  in: header
  name: wpNonce
  parameter: X-WP-Nonce
  sources:
  - openapi/effect-photonics-effect-v1-api-openapi.yml
  - openapi/effect-photonics-mcp-api-openapi.yml
  - openapi/effect-photonics-oembed-1-0-api-openapi.yml
  - openapi/effect-photonics-root-api-openapi.yml
  - openapi/effect-photonics-wp-abilities-v1-api-openapi.yml
  - openapi/effect-photonics-wp-v2-api-openapi.yml
  type: apiKey
- description: WordPress Application Passwords — HTTP Basic with a user-issued application password. The live discovery document at https://effectphotonics.com/wp-json/ names https://effectphotonics.com/wp-admin/authorize-application.php as the authorization endpoint.
  name: applicationPassword
  scheme: basic
  sources:
  - openapi/effect-photonics-effect-v1-api-openapi.yml
  - openapi/effect-photonics-mcp-api-openapi.yml
  - openapi/effect-photonics-oembed-1-0-api-openapi.yml
  - openapi/effect-photonics-root-api-openapi.yml
  - openapi/effect-photonics-wp-abilities-v1-api-openapi.yml
  - openapi/effect-photonics-wp-v2-api-openapi.yml
  type: http
slug: effect-photonics-authentication
source_filename: effect-photonics-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-12'\nmethod: derived\nsource: openapi/effect-photonics-effect-v1-api-openapi.yml, openapi/effect-photonics-mcp-api-openapi.yml,\n  openapi/effect-photonics-oembed-1-0-api-openapi.yml, openapi/effect-photonics-root-api-openapi.yml,\n  openapi/effect-photonics-wp-abilities-v1-api-openapi.yml, openapi/effect-photonics-wp-v2-api-openapi.yml\nsummary:\n  types:\n  - apiKey\n  - http\n  - oauth2\n  api_key_in:\n  - header\n  oauth2_flows:\n  - authorizationCode\nschemes:\n- name: mcpOAuth2\n  type: oauth2\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://effectphotonics.com/oauth/authorize\n    tokenUrl: https://effectphotonics.com/oauth/token\n    scopes: 1\n  description: OAuth 2.1 authorization-code + PKCE (S256), as advertised by the provider's RFC\n    8414 metadata at https://effectphotonics.com/.well-known/oauth-authorization-server (fetched\n    2026-08-12, HTTP 200). Guards the `mcp` namespace; the protected-resource metadata (RFC\n\
  \    9728) names https://effectphotonics.com/wp-json/mcp/mcp-oauth-server.\n  sources:\n  - openapi/effect-photonics-effect-v1-api-openapi.yml\n  - openapi/effect-photonics-mcp-api-openapi.yml\n  - openapi/effect-photonics-oembed-1-0-api-openapi.yml\n  - openapi/effect-photonics-root-api-openapi.yml\n  - openapi/effect-photonics-wp-abilities-v1-api-openapi.yml\n  - openapi/effect-photonics-wp-v2-api-openapi.yml\n- name: wpNonce\n  type: apiKey\n  in: header\n  parameter: X-WP-Nonce\n  description: WordPress cookie-authentication nonce. Advertised by the live server in its Access-Control-Allow-Headers\n    response header (Authorization, X-WP-Nonce, Content-Disposition, Content-MD5, Content-Type).\n  sources:\n  - openapi/effect-photonics-effect-v1-api-openapi.yml\n  - openapi/effect-photonics-mcp-api-openapi.yml\n  - openapi/effect-photonics-oembed-1-0-api-openapi.yml\n  - openapi/effect-photonics-root-api-openapi.yml\n  - openapi/effect-photonics-wp-abilities-v1-api-openapi.yml\n  - openapi/effect-photonics-wp-v2-api-openapi.yml\n\
  - name: applicationPassword\n  type: http\n  scheme: basic\n  description: WordPress Application Passwords — HTTP Basic with a user-issued application password.\n    The live discovery document at https://effectphotonics.com/wp-json/ names https://effectphotonics.com/wp-admin/authorize-application.php\n    as the authorization endpoint.\n  sources:\n  - openapi/effect-photonics-effect-v1-api-openapi.yml\n  - openapi/effect-photonics-mcp-api-openapi.yml\n  - openapi/effect-photonics-oembed-1-0-api-openapi.yml\n  - openapi/effect-photonics-root-api-openapi.yml\n  - openapi/effect-photonics-wp-abilities-v1-api-openapi.yml\n  - openapi/effect-photonics-wp-v2-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/effect-photonics/refs/heads/main/authentication/effect-photonics-authentication.yml
summary_line: apiKey/http/oauth2 · 3 schemes
tags:
- Company
- Photonics
- Optical Networking
- Optical Transceivers
- Photonic Integrated Circuits
- Semiconductors
- Telecommunications
- Data Center Interconnect
- Hardware
- Model Context Protocol
- WordPress
- Netherlands
---
