---
api_key_in: []
api_specs:
- filename: emerge-public-api-openapi.yml
  format: yaml
  label: Emerge Public API (Shipper API)
  slug: emerge-public-api-shipper-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/emerge/refs/heads/main/openapi/emerge-public-api-openapi.yml
- filename: emerge-carrier-api-openapi.yml
  format: yaml
  label: Emerge Carrier API
  slug: emerge-carrier-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/emerge/refs/heads/main/openapi/emerge-carrier-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: searched
name: Emerge Authentication
name_suffix: Authentication
oauth_flows: []
overview: Emerge secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Emerge
provider_slug: emerge
scheme_count: 1
schemes:
- header: 'Authorization: Bearer <token>'
  name: BearerAuth
  scheme: bearer
  sources:
  - openapi/emerge-carrier-api-openapi.yml
  - openapi/emerge-public-api-openapi.yml
  type: http
slug: emerge-authentication
source_filename: emerge-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-12'\nmethod: searched\nsource: openapi/emerge-carrier-api-openapi.yml, openapi/emerge-public-api-openapi.yml\ndocs: https://api-docs.emergemarket.io/\nsummary:\n  types:\n  - http\n  api_key_in: []\n  oauth2_flows: []\n  bearer_only: true\n  note: >-\n    Both Emerge APIs use a single `http`/`bearer` security scheme (`BearerAuth`). There is no\n    apiKey scheme, no OAuth 2.0 securityScheme, no OpenID Connect, and no mTLS. Tokens are minted at\n    proprietary login endpoints rather than an RFC 6749 token endpoint, and no scopes exist — a\n    token is all-or-nothing for the API it belongs to. There is consequently no `scopes/` artifact\n    for this provider.\nschemes:\n- name: BearerAuth\n  type: http\n  scheme: bearer\n  sources:\n  - openapi/emerge-carrier-api-openapi.yml\n  - openapi/emerge-public-api-openapi.yml\n  header: 'Authorization: Bearer <token>'\ntoken_acquisition:\n- api: Emerge Public API (Shipper API)\n  operation: POST /auth/login\n  security:\
  \ \"none (the operation declares `security: []`)\"\n  credentials:\n    kind: resource-owner password\n    fields: [user_name, password]\n    required: [user_name, password]\n    note: >-\n      The caller supplies an Emerge shipper user's own platform username and password. There is no\n      machine identity for the Shipper API — an integration authenticates as a human user account.\n  response_schema: 200_authentication_response\n  rate_limit: up to 20 requests per second, and lower during high-volume periods\n  errors: [403, 429, 500]\n- api: Emerge Public API (Shipper API)\n  operation: POST /auth/refresh\n  purpose: refresh an existing shipper access token without resending the password\n  errors: [400, 403]\n- api: Emerge Carrier API\n  operation: POST /auth/login/client_credentials\n  security: \"none (the operation declares `security: []`)\"\n  credentials:\n    kind: client credentials\n    fields: [client id, client secret]\n    note: >-\n      Issued to a Capacity/Integration\
  \ Provider during Capacity Link onboarding, alongside the\n      `relationship_identifiers` values that appear on rate_request events. Request access via\n      https://emergetech.zendesk.com/hc/en-us/requests/new?ticket_form_id=11470751569179\n  response_schema: 200_client_credential_authentication_response\n  errors: [400, 403]\ntoken_properties:\n  scopes: none\n  expiry: not documented in the OpenAPI response description\n  refresh: shipper only (POST /auth/refresh); no refresh path documented for carrier tokens\n  revocation: not documented\n  introspection: not documented\n  environment_binding:\n    mechanism: separate base host (api.emergemarket.io vs demo-api.emergemarket.dev)\n    key_prefix: none\n    note: >-\n      A token carries no visible marker of which environment it belongs to. Callers must track that\n      themselves — see sandbox/emerge-sandbox.yml.\ncallback_authentication:\n  surface: webhooks\n  mechanism: HTTP Basic on the subscriber's own endpoint\n  fields:\
  \ [authentication.is_enabled, authentication.username, authentication.password]\n  signature: none\n  note: >-\n    Emerge presents subscriber-supplied Basic credentials when delivering events. There is no HMAC\n    signature header, so TLS plus Basic is the entire verification story for inbound events. The\n    credentials are carried in cleartext in the webhook_object request/response shape.\n  detail: asyncapi/emerge-webhooks.yml\ndiscovery:\n  openid_configuration: absent (404 on every host)\n  oauth_authorization_server: absent (404 on every host)\n  oauth_protected_resource: absent (404 on every host)\n  detail: well-known/emerge-well-known.yml\ngaps:\n- Shipper API integrations authenticate as a named human user, not a service principal.\n- No scopes or least-privilege boundary between read and write operations.\n- Token lifetime, revocation and introspection are undocumented.\n- Webhook deliveries are not signed.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/emerge/refs/heads/main/authentication/emerge-authentication.yml
summary_line: http · 1 scheme
tags:
- freight
- logistics
- transportation
- supply-chain
- procurement
- trucking
- freight-marketplace
- transportation-management
- shipping
- rate-benchmarking
- webhooks
- b2b-marketplace
---
