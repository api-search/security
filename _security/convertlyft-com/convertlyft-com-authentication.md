---
anonymous_access: false
api_key_in: []
api_specs:
- filename: convertlyft-com-tools-api-openapi.yml
  format: yaml
  label: Convertlyft Tools API
  slug: convertlyft-com-tools-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/convertlyft-com/openapi/convertlyft-com-tools-api-openapi.yml
auth_types:
- http
- oauth2
description: ''
kind: authentication
layout: security
mechanism_count: 3
method: searched
name: Convertlyft Authentication
name_suffix: Authentication
oauth_flows: []
overview: Convertlyft secures its APIs with http and oauth2 across 3 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Convertlyft
provider_slug: convertlyft-com
scheme_count: 3
schemes:
- description: A cvl_pat_ personal access token, in the Authorization header only.
  header_only: true
  name: bearer
  notes: A cvl_pat_ token in a query string is refused with code token_in_query. "A credential lasts 90 days; then your client signs in again. There is no refresh token."
  scheme: bearer
  sources:
  - openapi/convertlyft-com-openapi.yml
  - https://convertlyft.com/api/public/llms
  token_format: cvl_pat_<12 hex>_<64 hex>
  type: http
- description: 'Headless: POST /api/tokens/device/code -> show user_code to a human -> poll POST /api/tokens/device/token (RFC 8628).'
  flow: device_code
  name: device-authorization
  poll: /api/tokens/device/token
  rfc: 8628
  sources:
  - https://convertlyft.com/api/public/llms
  start: /api/tokens/device/code
  type: oauth2
- description: 'For client builders: the server publishes its OAuth metadata at /.well-known/oauth-authorization-server. It supports dynamic client registration and client ID metadata documents, and requires PKCE with S256.'
  dynamic_client_registration: true
  flow: authorization_code
  metadata: /.well-known/oauth-authorization-server
  name: mcp-oauth
  pkce: S256
  sources:
  - https://convertlyft.com/developers
  type: oauth2
slug: convertlyft-com-authentication
source_filename: convertlyft-com-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-04'\nmethod: searched\nsource: https://convertlyft.com/api/public/llms\ndocs: https://convertlyft.com/api/public/llms\nsummary:\n  types:\n  - http\n  - oauth2\nschemes:\n- name: bearer\n  type: http\n  scheme: bearer\n  description: A cvl_pat_ personal access token, in the Authorization header only.\n  token_format: cvl_pat_<12 hex>_<64 hex>\n  header_only: true\n  notes: A cvl_pat_ token in a query string is refused with code token_in_query. \"A credential lasts 90 days; then your client signs in again. There is no refresh token.\"\n  sources:\n  - openapi/convertlyft-com-openapi.yml\n  - https://convertlyft.com/api/public/llms\n- name: device-authorization\n  type: oauth2\n  flow: device_code\n  rfc: 8628\n  start: /api/tokens/device/code\n  poll: /api/tokens/device/token\n  description: 'Headless: POST /api/tokens/device/code -> show user_code to a human -> poll POST /api/tokens/device/token (RFC 8628).'\n  sources:\n  - https://convertlyft.com/api/public/llms\n\
  - name: mcp-oauth\n  type: oauth2\n  flow: authorization_code\n  pkce: S256\n  metadata: /.well-known/oauth-authorization-server\n  dynamic_client_registration: true\n  description: 'For client builders: the server publishes its OAuth metadata at /.well-known/oauth-authorization-server. It supports dynamic client registration and client ID metadata documents, and requires\n    PKCE with S256.'\n  sources:\n  - https://convertlyft.com/developers\ndemo_credential: none\ndemo_credential_note: no demo credential is published in this document; there is no anonymous read, and you need a human once, to mint one\ndocs_also:\n- https://convertlyft.com/developers\n- https://convertlyft.com/.well-known/convertlyft-capabilities.json\n"
source_yaml_url: https://artifacts.apis.io/convertlyft-com/authentication/convertlyft-com-authentication.yml
summary_line: http/oauth2 · 3 schemes
tags:
- Company
- Web Analytics
- Conversion Rate Optimization
- Session Replay
- Heatmaps
- SEO
- Error Tracking
- MCP
---
