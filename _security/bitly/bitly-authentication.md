---
api_key_in: []
api_specs:
- filename: bitly-bitlinks-api-openapi.yml
  format: yaml
  label: Bitly Bitlinks API
  slug: bitly-bitlinks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bitly/refs/heads/main/openapi/bitly-bitlinks-api-openapi.yml
- filename: bitly-bsds-api-openapi.yml
  format: yaml
  label: Bitly BSDs API
  slug: bitly-bsds-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bitly/refs/heads/main/openapi/bitly-bsds-api-openapi.yml
- filename: bitly-campaigns-api-openapi.yml
  format: yaml
  label: Bitly Campaigns API
  slug: bitly-campaigns-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bitly/refs/heads/main/openapi/bitly-campaigns-api-openapi.yml
- filename: bitly-channels-api-openapi.yml
  format: yaml
  label: Bitly Channels API
  slug: bitly-channels-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bitly/refs/heads/main/openapi/bitly-channels-api-openapi.yml
- filename: bitly-custom-bitlinks-api-openapi.yml
  format: yaml
  label: Bitly Custom Bitlinks API
  slug: bitly-custom-bitlinks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bitly/refs/heads/main/openapi/bitly-custom-bitlinks-api-openapi.yml
- filename: bitly-group-metrics-api-openapi.yml
  format: yaml
  label: Bitly Group Metrics API
  slug: bitly-group-metrics-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bitly/refs/heads/main/openapi/bitly-group-metrics-api-openapi.yml
- filename: bitly-groups-api-openapi.yml
  format: yaml
  label: Bitly Groups API
  slug: bitly-groups-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bitly/refs/heads/main/openapi/bitly-groups-api-openapi.yml
- filename: bitly-metrics-api-openapi.yml
  format: yaml
  label: Bitly Metrics API
  slug: bitly-metrics-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bitly/refs/heads/main/openapi/bitly-metrics-api-openapi.yml
- filename: bitly-organizations-api-openapi.yml
  format: yaml
  label: Bitly Organizations API
  slug: bitly-organizations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bitly/refs/heads/main/openapi/bitly-organizations-api-openapi.yml
- filename: bitly-qr-codes-api-openapi.yml
  format: yaml
  label: Bitly QR Codes API
  slug: bitly-qr-codes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bitly/refs/heads/main/openapi/bitly-qr-codes-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Bitly Authentication
name_suffix: Authentication
oauth_flows: []
overview: Bitly secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Bitly
provider_slug: bitly
scheme_count: 1
schemes:
- description: 'Bearer token issued from Bitly account settings, or obtained via OAuth 2.0.

    Send as `Authorization: Bearer {token}`.'
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/bitly-openapi.yml
  type: http
slug: bitly-authentication
source_filename: bitly-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/bitly-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  description: |-\n    Bearer token issued from Bitly account settings, or obtained via OAuth 2.0.\n    Send as `Authorization: Bearer {token}`.\n  sources:\n  - openapi/bitly-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/bitly/refs/heads/main/authentication/bitly-authentication.yml
summary_line: http · 1 scheme
tags:
- Links
- URL Shortener
- QR Codes
- Analytics
- Marketing
---
