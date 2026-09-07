---
anonymous_access: false
api_key_in: []
api_specs:
- filename: scanverity-resolution-api-openapi.json
  format: json
  label: Scanverity Resolution API
  slug: scanverity-resolution-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/scanverity-resolution-api/refs/heads/main/openapi/scanverity-resolution-api-openapi.json
auth_types: []
description: Single-scheme HTTP Bearer authentication using opaque, reveal-once, account-scoped and environment-bound tokens. There is no OAuth 2.0, no OpenID Connect and no mutual TLS. Scopes are carried by the token itself rather than negotiated at an authorization server, and every scope is deny-by-default.
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Scanverity Resolution Api Authentication
name_suffix: Authentication
oauth_flows: []
overview: Scanverity Resolution API declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: Scanverity Resolution API
provider_slug: scanverity-resolution-api
scheme_count: 1
schemes:
- applied_to: all operations
  description: Reveal-once, account-scoped, environment-bound Resolution API token. Sent only in the Authorization header; query-string tokens are rejected with INVALID_REQUEST. Legacy svk_ Professional workspace tokens are explicitly rejected by this API.
  format: svr_live_... or svr_sandbox_...
  header: Authorization
  id: bearerToken
  in: header
  scheme: bearer
  token_prefixes:
  - environment: live
    note: Live tokens bill released assessments and are the only tokens accepted on the reconciled-usage routes.
    prefix: svr_live_
  - environment: sandbox
    note: Sandbox tokens read only the closed deterministic fixture catalog; every sandbox result is non-billable.
    prefix: svr_sandbox_
  - environment: rejected
    note: Legacy Professional workspace token. Intentionally rejected by the Resolution API.
    prefix: svk_
  type: http
slug: scanverity-resolution-api-authentication
source_filename: scanverity-resolution-api-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-09-04'\nmethod: searched\nsource: https://scanverity.com/resolution-api/docs\nderived_from: openapi/scanverity-resolution-api-openapi.json\nname: Scanverity Resolution API authentication profile\ndescription: >-\n  Single-scheme HTTP Bearer authentication using opaque, reveal-once, account-scoped and\n  environment-bound tokens. There is no OAuth 2.0, no OpenID Connect and no mutual TLS. Scopes are\n  carried by the token itself rather than negotiated at an authorization server, and every scope is\n  deny-by-default.\ndocs: https://scanverity.com/resolution-api/docs\nschemes:\n  - id: bearerToken\n    type: http\n    scheme: bearer\n    in: header\n    header: Authorization\n    format: \"svr_live_... or svr_sandbox_...\"\n    description: >-\n      Reveal-once, account-scoped, environment-bound Resolution API token. Sent only in the\n      Authorization header; query-string tokens are rejected with INVALID_REQUEST. Legacy svk_\n      Professional workspace\
  \ tokens are explicitly rejected by this API.\n    applied_to: all operations\n    token_prefixes:\n      - prefix: svr_live_\n        environment: live\n        note: Live tokens bill released assessments and are the only tokens accepted on the reconciled-usage routes.\n      - prefix: svr_sandbox_\n        environment: sandbox\n        note: Sandbox tokens read only the closed deterministic fixture catalog; every sandbox result is non-billable.\n      - prefix: svk_\n        environment: rejected\n        note: Legacy Professional workspace token. Intentionally rejected by the Resolution API.\nenvironments:\n  - name: live\n    token_prefix: svr_live_\n  - name: sandbox\n    token_prefix: svr_sandbox_\nscopes_model:\n  style: token-bound named scopes (not OAuth 2.0)\n  default: deny\n  reference: scopes/scanverity-resolution-api-scopes.yml\nfailure_modes:\n  - status: 401\n    code: INVALID_TOKEN\n    note: >-\n      Unknown, malformed, expired and revoked credentials deliberately share\
  \ one indistinguishable\n      response so a caller cannot enumerate token state.\n  - status: 403\n    code: INSUFFICIENT_SCOPE\n    note: The credential is valid but does not carry the scope the operation requires.\n  - status: 400\n    code: INVALID_REQUEST\n    note: Returned when a token is supplied in the URL rather than the Authorization header.\nnotes:\n  - Token secrets are revealed once at creation and are never returned by later reads.\n  - Access is private beta and feature-gated; a valid token still requires an entitled, allowlisted account.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/scanverity-resolution-api/refs/heads/main/authentication/scanverity-resolution-api-authentication.yml
summary_line: 1 scheme
tags:
- Prediction Markets
- Resolution Risk
- Market Intelligence
- Due Diligence
- Webhooks
- OpenAPI
- Fintech
- Risk Analytics
- Polymarket
- Event Contracts
- Agent Ready
---
