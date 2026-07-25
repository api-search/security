---
api_key_in:
- header
api_specs:
- filename: punchh-check-in-api-openapi.yml
  format: yaml
  label: Punchh Check-In API
  slug: punchh-check-in-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/punchh/refs/heads/main/openapi/punchh-check-in-api-openapi.yml
- filename: punchh-check-ins-api-openapi.yml
  format: yaml
  label: Punchh Check-Ins API
  slug: punchh-check-ins-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/punchh/refs/heads/main/openapi/punchh-check-ins-api-openapi.yml
- filename: punchh-configuration-api-openapi.yml
  format: yaml
  label: Punchh Configuration API
  slug: punchh-configuration-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/punchh/refs/heads/main/openapi/punchh-configuration-api-openapi.yml
- filename: punchh-offers-api-openapi.yml
  format: yaml
  label: Punchh Offers API
  slug: punchh-offers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/punchh/refs/heads/main/openapi/punchh-offers-api-openapi.yml
- filename: punchh-receipts-api-openapi.yml
  format: yaml
  label: Punchh Receipts API
  slug: punchh-receipts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/punchh/refs/heads/main/openapi/punchh-receipts-api-openapi.yml
- filename: punchh-redemptions-api-openapi.yml
  format: yaml
  label: Punchh Redemptions API
  slug: punchh-redemptions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/punchh/refs/heads/main/openapi/punchh-redemptions-api-openapi.yml
- filename: punchh-users-api-openapi.yml
  format: yaml
  label: Punchh Users API
  slug: punchh-users-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/punchh/refs/heads/main/openapi/punchh-users-api-openapi.yml
auth_types:
- apiKey
- http
description: ''
kind: authentication
layout: security
method: derived
name: Punchh Authentication
name_suffix: Authentication
oauth_flows: []
overview: Punchh secures its APIs with apiKey and http across 3 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Punchh
provider_slug: punchh
scheme_count: 3
schemes:
- description: Bearer access token obtained via Sign In. Calls must also include an `x-pch-digest` HMAC-SHA256 signature header and a `punchh-app-device-id` header.
  name: PunchhBearer
  scheme: bearer
  sources:
  - openapi/punchh-mobile-openapi.yml
  - openapi/punchh-online-ordering-openapi.yml
  - openapi/punchh-platform-functions-openapi.yml
  type: http
- description: HMAC-SHA256 request signature. Unauthenticated mobile calls also pass the business OAuth `client` id in the request body.
  in: header
  name: PunchhDigest
  parameter: x-pch-digest
  sources:
  - openapi/punchh-mobile-openapi.yml
  type: apiKey
- description: Token pair credential of the form `Token token=LOCATION_KEY, btoken=BUSINESS_KEY`. Requests must also send a structured `User-Agent` of the form `IntegratorName/IntegrationType/VersionNumber`.
  in: header
  name: PunchhPosToken
  parameter: Authorization
  sources:
  - openapi/punchh-pos-openapi.yml
  type: apiKey
slug: punchh-authentication
source_filename: punchh-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/punchh-mobile-openapi.yml, openapi/punchh-online-ordering-openapi.yml, openapi/punchh-platform-functions-openapi.yml,\n  openapi/punchh-pos-openapi.yml\nsummary:\n  types:\n  - apiKey\n  - http\n  api_key_in:\n  - header\nschemes:\n- name: PunchhBearer\n  type: http\n  scheme: bearer\n  description: Bearer access token obtained via Sign In. Calls must also include an `x-pch-digest`\n    HMAC-SHA256 signature header and a `punchh-app-device-id` header.\n  sources:\n  - openapi/punchh-mobile-openapi.yml\n  - openapi/punchh-online-ordering-openapi.yml\n  - openapi/punchh-platform-functions-openapi.yml\n- name: PunchhDigest\n  type: apiKey\n  in: header\n  parameter: x-pch-digest\n  description: HMAC-SHA256 request signature. Unauthenticated mobile calls also pass the business\n    OAuth `client` id in the request body.\n  sources:\n  - openapi/punchh-mobile-openapi.yml\n- name: PunchhPosToken\n  type: apiKey\n  in: header\n\
  \  parameter: Authorization\n  description: Token pair credential of the form `Token token=LOCATION_KEY, btoken=BUSINESS_KEY`.\n    Requests must also send a structured `User-Agent` of the form `IntegratorName/IntegrationType/VersionNumber`.\n  sources:\n  - openapi/punchh-pos-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/punchh/refs/heads/main/authentication/punchh-authentication.yml
summary_line: apiKey/http · 3 schemes
tags:
- Restaurant
- Loyalty
- Marketing
- Guest Engagement
- Online Ordering
- Mobile
- Point Of Sale
- Webhooks
---
