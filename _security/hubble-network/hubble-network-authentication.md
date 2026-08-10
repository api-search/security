---
api_key_in:
- header
api_specs:
- filename: hubble-network-api-keys-api-openapi.yml
  format: yaml
  label: Hubble Network API Keys API
  slug: hubble-network-api-keys-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hubble-network/refs/heads/main/openapi/hubble-network-api-keys-api-openapi.yml
- filename: hubble-network-billing-api-openapi.yml
  format: yaml
  label: Hubble Network Billing API
  slug: hubble-network-billing-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hubble-network/refs/heads/main/openapi/hubble-network-billing-api-openapi.yml
- filename: hubble-network-devices-api-openapi.yml
  format: yaml
  label: Hubble Network Devices API
  slug: hubble-network-devices-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hubble-network/refs/heads/main/openapi/hubble-network-devices-api-openapi.yml
- filename: hubble-network-organizations-api-openapi.yml
  format: yaml
  label: Hubble Network Organizations API
  slug: hubble-network-organizations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hubble-network/refs/heads/main/openapi/hubble-network-organizations-api-openapi.yml
- filename: hubble-network-packet-webhooks-api-openapi.yml
  format: yaml
  label: Hubble Network Packet Webhooks API
  slug: hubble-network-packet-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hubble-network/refs/heads/main/openapi/hubble-network-packet-webhooks-api-openapi.yml
- filename: hubble-network-packets-api-openapi.yml
  format: yaml
  label: Hubble Network Packets API
  slug: hubble-network-packets-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hubble-network/refs/heads/main/openapi/hubble-network-packets-api-openapi.yml
- filename: hubble-network-platform-metrics-api-openapi.yml
  format: yaml
  label: Hubble Network Platform Metrics API
  slug: hubble-network-platform-metrics-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hubble-network/refs/heads/main/openapi/hubble-network-platform-metrics-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: searched
name: Hubble Network Authentication
name_suffix: Authentication
oauth_flows: []
overview: Hubble Network secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Hubble Network
provider_slug: hubble-network
scheme_count: 1
schemes:
- applied: globally (root security requirement) to all 39 operations
  bearerFormat: JWT
  header: 'Authorization: Bearer <api-key-jwt>'
  issuance: Hubble Dashboard > Developer Tools > API Tokens. Keys are named, given an expiration date, and optionally restricted to a scope set. A key created with no scopes receives ALL scopes (admin-level access). Tokens cannot be retrieved after creation.
  name: BearerAuth
  rotation: Keys carry a calendar expiration (apiKeyExpiration); update-api-key can change name, scopes and expiry; delete-api-key revokes.
  scheme: bearer
  sources:
  - openapi/hubble-network-platform-openapi.yml
  type: http
  validation_endpoint: GET /v1/org/{org_id}/check (operationId validate-api-key)
slug: hubble-network-authentication
source_filename: hubble-network-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-04'\nmethod: searched\nsource: openapi/hubble-network-platform-openapi.yml\ndocs: https://hubble.com/docs/api-specification/hubble-platform-api\nsummary:\n  types:\n  - http\n  http_schemes:\n  - bearer\n  bearer_formats:\n  - JWT\n  api_key_in:\n  - header\n  oauth2_flows: []\n  model: Organization-scoped API key presented as a JWT bearer token, with 16 granular authorization scopes.\nschemes:\n- name: BearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  applied: globally (root security requirement) to all 39 operations\n  header: 'Authorization: Bearer <api-key-jwt>'\n  issuance: Hubble Dashboard > Developer Tools > API Tokens. Keys are named, given an expiration date,\n    and optionally restricted to a scope set. A key created with no scopes receives ALL scopes (admin-level\n    access). Tokens cannot be retrieved after creation.\n  validation_endpoint: GET /v1/org/{org_id}/check (operationId validate-api-key)\n  rotation: Keys carry a\
  \ calendar expiration (apiKeyExpiration); update-api-key can change name, scopes\n    and expiry; delete-api-key revokes.\n  sources:\n  - openapi/hubble-network-platform-openapi.yml\ntenancy:\n  parameter: org_id\n  in: path\n  required: true\n  note: Every operation is scoped to an organization UUID carried in the path. The org_id is shown in\n    the Dashboard under Developer Tools > API Tokens or Organization Settings.\nscopes:\n  model: api-key-scopes\n  count: 16\n  artifact: scopes/hubble-network-scopes.yml\n  enumeration_endpoint: GET /v1/org/{org_id}/key_scopes (operationId list-key-scopes)\n  note: Not OAuth 2.0 scopes — these are permission scopes attached to an organization API key. Every\n    endpoint documents its Required Scope.\nwebhook_authentication:\n  header: HTTP-X-HUBBLE-TOKEN\n  note: Outbound packet webhooks carry a shared secret in the HTTP-X-HUBBLE-TOKEN header; the receiver\n    must validate it. There is no HMAC signature scheme.\nsso:\n  available: Enterprise\
  \ plan only\n  source: https://hubble.com/pricing\nx-evidence:\n- url: https://hubble.com/docs/api-specification/hubble-platform-api\n  http_status: 200\n  fetched: '2026-08-04'\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/hubble-network/refs/heads/main/authentication/hubble-network-authentication.yml
summary_line: http · 1 scheme
tags:
- Company
- IoT
- Bluetooth
- Satellite
- Connectivity
- Asset Tracking
- Devices
- Networks
- Telemetry
- Logistics
---
