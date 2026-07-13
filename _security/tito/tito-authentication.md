---
api_key_in: []
api_specs:
- filename: tito-openapi.yml
  format: yaml
  label: Tito Events API
  slug: tito-events-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tito/refs/heads/main/openapi/tito-openapi.yml
- filename: tito-openapi.yml
  format: yaml
  label: Tito Releases API
  slug: tito-releases-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tito/refs/heads/main/openapi/tito-openapi.yml
- filename: tito-openapi.yml
  format: yaml
  label: Tito Tickets API
  slug: tito-tickets-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tito/refs/heads/main/openapi/tito-openapi.yml
- filename: tito-openapi.yml
  format: yaml
  label: Tito Registrations API
  slug: tito-registrations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tito/refs/heads/main/openapi/tito-openapi.yml
- filename: tito-openapi.yml
  format: yaml
  label: Tito Discount Codes API
  slug: tito-discount-codes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tito/refs/heads/main/openapi/tito-openapi.yml
- filename: tito-openapi.yml
  format: yaml
  label: Tito Activities API
  slug: tito-activities-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tito/refs/heads/main/openapi/tito-openapi.yml
- filename: tito-openapi.yml
  format: yaml
  label: Tito Check-in Lists API
  slug: tito-check-in-lists-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tito/refs/heads/main/openapi/tito-openapi.yml
- filename: tito-openapi.yml
  format: yaml
  label: Tito Refunds API
  slug: tito-refunds-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tito/refs/heads/main/openapi/tito-openapi.yml
- filename: tito-openapi.yml
  format: yaml
  label: Tito Webhook Endpoints API
  slug: tito-webhook-endpoints-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tito/refs/heads/main/openapi/tito-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: documented
name: Tito Authentication
name_suffix: Authentication
oauth_flows: []
overview: Tito secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Tito
provider_slug: tito
scheme_count: 1
schemes:
- description: 'The Tito Admin API authenticates with a secret API token. Generate a token by signing in at https://id.tito.io (api-access-tokens) and selecting "Generate New Token". Only secret token types are valid for the private Admin API, and each token is scoped to a live or test mode (test tokens read and write only test data). The token is sent in the Authorization header as "Token token=YOUR-API-TOKEN", and every request must also send "Accept: application/json". A compromised token can be revoked and regenerated at https://id.tito.io/api-access-tokens. The GET /hello endpoint confirms a token is valid and lists the accounts it can access. Note the separate Tito Check-in API (https://checkin.tito.io) is unauthenticated and instead scopes access by including a Check-in List slug in the URL.'
  format: Token token=YOUR-API-TOKEN
  in: header
  name: titoToken
  parameterName: Authorization
  sources:
  - https://ti.to/docs/api/admin/3.0
  - openapi/tito-openapi.yml
  type: apiKey
slug: tito-authentication
source_filename: tito-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-12'\nmethod: documented\nsource: openapi/tito-openapi.yml\nsummary:\n  types:\n  - apiKey\nschemes:\n- name: titoToken\n  type: apiKey\n  in: header\n  parameterName: Authorization\n  format: 'Token token=YOUR-API-TOKEN'\n  description: >-\n    The Tito Admin API authenticates with a secret API token. Generate a token\n    by signing in at https://id.tito.io (api-access-tokens) and selecting\n    \"Generate New Token\". Only secret token types are valid for the private\n    Admin API, and each token is scoped to a live or test mode (test tokens\n    read and write only test data). The token is sent in the Authorization\n    header as \"Token token=YOUR-API-TOKEN\", and every request must also send\n    \"Accept: application/json\". A compromised token can be revoked and\n    regenerated at https://id.tito.io/api-access-tokens. The GET /hello endpoint\n    confirms a token is valid and lists the accounts it can access. Note the\n    separate Tito Check-in\
  \ API (https://checkin.tito.io) is unauthenticated and\n    instead scopes access by including a Check-in List slug in the URL.\n  sources:\n  - https://ti.to/docs/api/admin/3.0\n  - openapi/tito-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/tito/refs/heads/main/authentication/tito-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Event Ticketing
- Events
- Registration
- Ticketing
- Conferences
- Event Management
- Attendees
- Webhooks
- SaaS
---
