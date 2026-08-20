---
api_key_in:
- header
api_specs:
- filename: skipodds-openapi.yml
  format: yaml
  label: SkipOdds REST API
  slug: skipodds-rest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/skipodds/refs/heads/main/openapi/skipodds-openapi.yml
auth_types:
- apiKey
- http
description: ''
kind: authentication
layout: security
method: searched
name: Skipodds Authentication
name_suffix: Authentication
oauth_flows: []
overview: SkipOdds secures its APIs with apiKey and http across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: SkipOdds
provider_slug: skipodds
scheme_count: 2
schemes:
- applies_to: all 11 operations (global security)
  description: 'Preferred. Send the API key as `Authorization: Bearer <key>`.'
  name: BearerAuth
  scheme: bearer
  sources:
  - openapi/skipodds-openapi.yml
  type: http
- applies_to: all 11 operations (global security)
  description: Accepted for existing integrations.
  in: header
  name: ApiKeyHeader
  parameter: x-api-key
  sources:
  - openapi/skipodds-openapi.yml
  type: apiKey
slug: skipodds-authentication
source_filename: skipodds-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-11'\nmethod: searched\nsource: openapi/skipodds-openapi.yml\ndocs: https://skipodds.com/docs\nsummary:\n  types:\n    - apiKey\n    - http\n  api_key_in:\n    - header\n  oauth2_flows: []\n  model: static-api-key\n  note: >-\n    One credential, two accepted transports. Both schemes carry the SAME static API key — Bearer is the\n    preferred transport and x-api-key is retained for existing integrations. There is no OAuth, no token\n    exchange, no refresh, no expiry, and no scopes, so no scopes/ artifact is written for this provider.\nschemes:\n  - name: BearerAuth\n    type: http\n    scheme: bearer\n    description: 'Preferred. Send the API key as `Authorization: Bearer <key>`.'\n    sources:\n      - openapi/skipodds-openapi.yml\n    applies_to: all 11 operations (global security)\n  - name: ApiKeyHeader\n    type: apiKey\n    in: header\n    parameter: x-api-key\n    description: Accepted for existing integrations.\n    sources:\n      - openapi/skipodds-openapi.yml\n\
  \    applies_to: all 11 operations (global security)\nprohibited_transports:\n  - transport: query string\n    statement: >-\n      \"Never put a key in the query string\" — stated in the OpenAPI info.description, on every docs\n      page header, and again on https://skipodds.com/mcp (\"anything in a link is in somebody's logs\").\nanonymous_access:\n  supported: true\n  mechanism: >-\n    Calls with no credential fall onto a published shared demo key, skipodds-demo-2026, at 100\n    requests/day shared across ALL anonymous callers. This applies to both the REST API and the MCP\n    server at https://skipodds.com/mcp, which was confirmed to answer tools/list with no Authorization\n    header at all.\n  see: sandbox/skipodds-sandbox.yml\nkey_issuance:\n  free_personal_key: https://skipodds.com/#free\n  method: Self-serve form on the homepage (POSTs to /free-key); email delivery via Resend. No card.\n  paid_keys: Issued on Stripe checkout; the subscriber email comes from Stripe.\n  rotation:\
  \ not documented\n  revocation: >-\n    The terms reserve the right to throttle, suspend, or revoke keys that exceed limits or attempt to\n    circumvent quotas. No self-serve rotation or revocation surface is published.\n  sharing: 'Keys are personal to the subscriber and may not be shared or resold (https://skipodds.com/terms).'\nfailure_mode:\n  status: 401\n  body: '{\"error\": \"invalid_api_key\"}'\n  www_authenticate_header: false\n  note: >-\n    No WWW-Authenticate challenge is returned, so a 401 is not discoverable by an RFC 6750 client — the\n    caller has to parse the body.\ngaps:\n  - No OAuth 2.0 or OIDC; /.well-known/oauth-authorization-server and /.well-known/openid-configuration both 404.\n  - No scopes or permission model — a key is all-or-nothing across every operation.\n  - No key expiry, rotation endpoint, or published rotation guidance.\n  - No mTLS, no request signing, no IP allow-listing.\n  - The OpenAPI redundantly declares x-api-key as an optional header PARAMETER\
  \ on every operation in addition to the securityScheme, which will produce a duplicate argument in generated clients.\ncross_links:\n  conventions: conventions/skipodds-conventions.yml\n  sandbox: sandbox/skipodds-sandbox.yml\n  rate_limits: rate-limits/skipodds-rate-limits.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/skipodds/refs/heads/main/authentication/skipodds-authentication.yml
summary_line: apiKey/http · 2 schemes
tags:
- Sports
- Odds
- probabilities
- Betting Data
- de-vig
- Sports Data
- Real-Time
- Webhook
- Sports Betting
- MCP
- Agent Ready
- Market Data
---
