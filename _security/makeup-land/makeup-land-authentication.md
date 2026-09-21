---
anonymous_access: false
api_key_in:
- query
api_specs:
- filename: makeup-land-openapi.yml
  format: yaml
  label: makeup.land V1 API
  slug: makeup-land-v1-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/makeup-land/refs/heads/main/openapi/makeup-land-openapi.yml
auth_types:
- apiKey
- http
description: ''
kind: authentication
layout: security
mechanism_count: 2
method: searched
name: Makeup Land Authentication
name_suffix: Authentication
oauth_flows: []
overview: א. ט. הפקות בע״מ / A.T. Hafakot Ltd. secures its APIs with apiKey and http across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: א. ט. הפקות בע״מ / A.T. Hafakot Ltd.
provider_slug: makeup-land
scheme_count: 2
schemes:
- agent_auth: RFC 8414 metadata carries agent_auth {register_uri mailto:info@makeup.land, identity_types_supported [identity_assertion], identity_assertion.methods [email_manual], credentials_issued [api_key]} — the WorkOS auth.md pattern; the skill file is saved verbatim at skills/makeup-land-auth.md.
  bearerFormat: ml_<hex24>
  description: API bearer token issued under `api_tokens`. Prefix `ml_` is required. Per-token scope and `read_only` flag govern endpoint + write access.
  discovery:
  - https://makeup.land/.well-known/oauth-protected-resource
  - https://makeup.land/.well-known/oauth-authorization-server
  expiry: Tokens do not expire automatically.
  flags:
  - read_only
  issuance: 'Email info@makeup.land (auth.md) or shop@makeup.land (llms-api.txt, MCP README) with operator identity, use case, desired scope and read_only preference; an admin issues the token from the api_tokens table. "Median turnaround: a few business hours during Israel working hours. There is no SLA today."'
  name: bearerAuth
  observed: GET /api/v1/brands without a token -> 401 {"error":"Unauthorized"} (2026-09-19)
  revocation: Manual by email with the token prefix; no self-service revocation endpoint. Revoked tokens return 401 unauthorized.
  rotation: None in-band — on a 401 treat the credential as invalid, do not auto-retry, request a new token by email.
  scheme: bearer
  scopes:
  - full
  - register
  - giftcards
  - proposals
  sources:
  - openapi/makeup-land-openapi.yml
  type: http
- description: Phone number in E.164 format (e.g. `+972501234567`) that selects which customer's resources to return. **NOT a credential** — endpoints that accept this also REQUIRE `bearerAuth`. The bearer authenticates the calling partner; the phone selects the customer. For POST/PATCH cart-mutation endpoints, the phone goes in the JSON body instead of the query string.
  in: query
  location_rule: ?phone= query for GET/DELETE; phone in the JSON body for POST/PATCH cart mutations
  name: phoneIdentifier
  observed: 'The provider: "A bearer without phone is rejected with 400 phone parameter required; a phone without bearer is rejected with 401 Unauthorized."'
  parameter: phone
  selector_not_credential: true
  sources:
  - openapi/makeup-land-openapi.yml
  type: apiKey
slug: makeup-land-authentication
source_filename: makeup-land-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-09-19'\nmethod: searched\nsource: openapi/makeup-land-openapi.yml (securitySchemes) upgraded from https://makeup.land/auth.md, https://makeup.land/llms-full.txt,\n  the RFC 8414/9728 metadata and live 401/400 responses on 2026-09-19\nsummary:\n  types:\n  - apiKey\n  - http\n  api_key_in:\n  - query\n  oauth2_flows: []\n  issuance: manual — bearer issued by a human over email; no self-serve signup, no OAuth flow, no token expiry,\n    manual revocation\n  anonymous_surface:\n  - validateGiftCard\n  - listProducts with catalog filters only\n  - MCP initialize / tools/list / list_products / validate_gift_card\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: ml_<hex24>\n  description: API bearer token issued under `api_tokens`. Prefix `ml_` is required. Per-token scope and `read_only`\n    flag govern endpoint + write access.\n  sources:\n  - openapi/makeup-land-openapi.yml\n  issuance: 'Email info@makeup.land (auth.md) or shop@makeup.land\
  \ (llms-api.txt, MCP README) with operator identity,\n    use case, desired scope and read_only preference; an admin issues the token from the api_tokens table. \"Median\n    turnaround: a few business hours during Israel working hours. There is no SLA today.\"'\n  scopes:\n  - full\n  - register\n  - giftcards\n  - proposals\n  flags:\n  - read_only\n  expiry: Tokens do not expire automatically.\n  revocation: Manual by email with the token prefix; no self-service revocation endpoint. Revoked tokens return\n    401 unauthorized.\n  rotation: None in-band — on a 401 treat the credential as invalid, do not auto-retry, request a new token by email.\n  discovery:\n  - https://makeup.land/.well-known/oauth-protected-resource\n  - https://makeup.land/.well-known/oauth-authorization-server\n  agent_auth: RFC 8414 metadata carries agent_auth {register_uri mailto:info@makeup.land, identity_types_supported\n    [identity_assertion], identity_assertion.methods [email_manual], credentials_issued\
  \ [api_key]} — the WorkOS\n    auth.md pattern; the skill file is saved verbatim at skills/makeup-land-auth.md.\n  observed: GET /api/v1/brands without a token -> 401 {\"error\":\"Unauthorized\"} (2026-09-19)\n- name: phoneIdentifier\n  type: apiKey\n  in: query\n  parameter: phone\n  description: Phone number in E.164 format (e.g. `+972501234567`) that selects which customer's resources to return.\n    **NOT a credential** — endpoints that accept this also REQUIRE `bearerAuth`. The bearer authenticates the calling\n    partner; the phone selects the customer. For POST/PATCH cart-mutation endpoints, the phone goes in the JSON\n    body instead of the query string.\n  sources:\n  - openapi/makeup-land-openapi.yml\n  selector_not_credential: true\n  location_rule: ?phone= query for GET/DELETE; phone in the JSON body for POST/PATCH cart mutations\n  observed: 'The provider: \"A bearer without phone is rejected with 400 phone parameter required; a phone without\n    bearer is rejected with\
  \ 401 Unauthorized.\"'\ndocs: https://makeup.land/auth.md\nerror_codes:\n  '401': unauthorized\n  '403':\n  - scope_mismatch\n  - read_only_token\n  detail: errors/makeup-land-problem-types.yml\nscopes_detail: scopes/makeup-land-scopes.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/makeup-land/refs/heads/main/authentication/makeup-land-authentication.yml
summary_line: apiKey/http · 2 schemes
tags:
- Cosmetics
- Beauty
- Retail
- E-Commerce
- Shopping
- Loyalty
- Gift Cards
- Product Search
- Agentic Commerce
- MCP
- agent-native
- Israel
---
