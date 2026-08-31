---
api_key_in:
- header
api_specs:
- filename: lucra-sports-health-api-openapi.yml
  format: yaml
  label: Lucra Sports Health API
  slug: lucra-sports-health-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lucra-sports/refs/heads/main/openapi/lucra-sports-health-api-openapi.yml
- filename: lucra-sports-locations-api-openapi.yml
  format: yaml
  label: Lucra Sports Locations API
  slug: lucra-sports-locations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lucra-sports/refs/heads/main/openapi/lucra-sports-locations-api-openapi.yml
- filename: lucra-sports-recreational-games-api-openapi.yml
  format: yaml
  label: Lucra Sports Recreational Games API
  slug: lucra-sports-recreational-games-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lucra-sports/refs/heads/main/openapi/lucra-sports-recreational-games-api-openapi.yml
- filename: lucra-sports-states-api-openapi.yml
  format: yaml
  label: Lucra Sports States API
  slug: lucra-sports-states-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lucra-sports/refs/heads/main/openapi/lucra-sports-states-api-openapi.yml
- filename: lucra-sports-tenanttaggroups-api-openapi.yml
  format: yaml
  label: Lucra Sports Tenant Tag Groups API
  slug: lucra-sports-tenanttaggroups-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lucra-sports/refs/heads/main/openapi/lucra-sports-tenanttaggroups-api-openapi.yml
- filename: lucra-sports-tournaments-api-openapi.yml
  format: yaml
  label: Lucra Sports Tournaments API
  slug: lucra-sports-tournaments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lucra-sports/refs/heads/main/openapi/lucra-sports-tournaments-api-openapi.yml
- filename: lucra-sports-tournaments-legacy-api-openapi.yml
  format: yaml
  label: Lucra Sports Tournaments (Legacy) API
  slug: lucra-sports-tournaments-legacy-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lucra-sports/refs/heads/main/openapi/lucra-sports-tournaments-legacy-api-openapi.yml
- filename: lucra-sports-user-score-api-openapi.yml
  format: yaml
  label: Lucra Sports User Score API
  slug: lucra-sports-user-score-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lucra-sports/refs/heads/main/openapi/lucra-sports-user-score-api-openapi.yml
- filename: lucra-sports-webhooks-api-openapi.yml
  format: yaml
  label: Lucra Sports Webhooks API
  slug: lucra-sports-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lucra-sports/refs/heads/main/openapi/lucra-sports-webhooks-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: searched
name: Lucra Sports Authentication
name_suffix: Authentication
oauth_flows: []
overview: Lucra Sports secures its APIs with apiKey across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Lucra Sports
provider_slug: lucra-sports
scheme_count: 2
schemes:
- applies_to: https://forge.lucrasports.com
  description: Tenant API key. The only supported authentication on the Forge gateway.
  in: header
  name: X-Lucra-Api-Key
  parameter: X-Lucra-Api-Key
  sources:
  - openapi/lucra-sports-forge-openapi.json
  - https://docs.lucrasports.com/lucra-sdk/sdks-and-apis/api-reference.md
  type: apiKey
- applies_to: https://api.lucrasports.com
  description: 'The legacy api.lucrasports.com REST surface accepted the key as an `apiKey` query parameter (and in the request body for webhook config calls). Forge explicitly removed this: "Unlike the legacy API, query parameter and request body authentication are not supported."'
  in: query
  name: apiKey (query parameter)
  parameter: apiKey
  sources:
  - https://docs.lucrasports.com/lucra-sdk/server-to-server/api-integration.md
  - https://docs.lucrasports.com/lucra-sdk/sdks-and-apis/api-reference/legacy/1.0_api_setup.md
  status: legacy
  type: apiKey
slug: lucra-sports-authentication
source_filename: lucra-sports-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-25'\nmethod: searched\nsource: https://docs.lucrasports.com/lucra-sdk/readme/whats-included/lucra-api-keys.md\ndocs: https://docs.lucrasports.com/lucra-sdk/readme/whats-included/lucra-api-keys\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\n  oauth2: false\n  openid_connect: false\n  mutual_tls: false\n  note: >-\n    Lucra authenticates every server-to-server call with a tenant-scoped API key. There is no OAuth\n    flow and no self-service key management: keys are provisioned by a Lucra representative per\n    tenant per environment, and the docs state key generation and rotation are not currently\n    self-service. End-user identity inside the SDK is handled separately by Auth0 (SMS login) and is\n    not part of the partner API contract.\nschemes:\n- name: X-Lucra-Api-Key\n  type: apiKey\n  in: header\n  parameter: X-Lucra-Api-Key\n  description: Tenant API key. The only supported authentication on the Forge gateway.\n  applies_to: https://forge.lucrasports.com\n\
  \  sources:\n  - openapi/lucra-sports-forge-openapi.json\n  - https://docs.lucrasports.com/lucra-sdk/sdks-and-apis/api-reference.md\n- name: apiKey (query parameter)\n  type: apiKey\n  in: query\n  parameter: apiKey\n  status: legacy\n  description: >-\n    The legacy api.lucrasports.com REST surface accepted the key as an `apiKey` query parameter (and\n    in the request body for webhook config calls). Forge explicitly removed this: \"Unlike the legacy\n    API, query parameter and request body authentication are not supported.\"\n  applies_to: https://api.lucrasports.com\n  sources:\n  - https://docs.lucrasports.com/lucra-sdk/server-to-server/api-integration.md\n  - https://docs.lucrasports.com/lucra-sdk/sdks-and-apis/api-reference/legacy/1.0_api_setup.md\nkey_types:\n- name: BACKEND\n  usage: Server-side API calls; supplied in the X-Lucra-Api-Key header.\n- name: WEB\n  usage: Lucra Web (JavaScript) SDK initialization; paired with a tenantId.\n- name: MOBILE\n  usage: Lucra iOS, Android\
  \ and React Native SDK initialization, provided at runtime.\nenvironments:\n- name: sandbox\n  description: Development and testing keys; separate credentials from production.\n- name: production\n  description: Live keys only.\nprovisioning:\n  self_service: false\n  note: >-\n    \"Keys must be provided by your Lucra representative. API key generation and management is not\n    currently supported.\" Partners are onboarded through a sales/solutions conversation, not a\n    developer signup.\nrotation:\n  self_service: false\n  guidance: Contact the Lucra team if a key is suspected to be compromised.\nwebhook_authentication:\n  outbound_signature_header: X-Lucra-Signature\n  algorithm: HMAC-SHA256 (hex digest, sha256= prefixed)\n  secret_distribution: Per-webhook shared secret issued by a Lucra representative out of band.\n  source: https://docs.lucrasports.com/lucra-sdk/server-to-server/webhook-subscriptions/request-verification.md\ngraphql_surface:\n  endpoint: https://api.lucrasports.com/v1/graphql\n\
  \  probed: '2026-08-25'\n  http_status: 200\n  introspection: disabled\n  response: 'introspection is disabled for role: \"anonymous\"'\n  note: >-\n    A Hasura GraphQL endpoint backs the client SDKs and answers anonymously with an\n    introspection-disabled error. It is not a documented partner surface and no SDL could be\n    retrieved; nothing about its schema is recorded here.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/lucra-sports/refs/heads/main/authentication/lucra-sports-authentication.yml
summary_line: apiKey · 2 schemes
tags:
- Gaming
- Sports
- Gamification
- Loyalty
- Tournaments
- Contests
- Payments
- Wagering
- Embedded Finance
- SDKs
- Webhooks
- Compliance
---
