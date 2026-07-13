---
api_key_in:
- header
api_specs:
- filename: hotelbeds-openapi.yml
  format: yaml
  label: Hotel Booking API
  slug: hotel-booking-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hotelbeds/refs/heads/main/openapi/hotelbeds-openapi.yml
- filename: hotelbeds-openapi.yml
  format: yaml
  label: Hotel Content API
  slug: hotel-content-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hotelbeds/refs/heads/main/openapi/hotelbeds-openapi.yml
- filename: hotelbeds-openapi.yml
  format: yaml
  label: Cache Rates API
  slug: cache-rates-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hotelbeds/refs/heads/main/openapi/hotelbeds-openapi.yml
- filename: hotelbeds-openapi.yml
  format: yaml
  label: Activities API
  slug: activities-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hotelbeds/refs/heads/main/openapi/hotelbeds-openapi.yml
- filename: hotelbeds-openapi.yml
  format: yaml
  label: Transfers API
  slug: transfers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hotelbeds/refs/heads/main/openapi/hotelbeds-openapi.yml
- filename: hotelbeds-openapi.yml
  format: yaml
  label: Webhooks
  slug: webhooks
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hotelbeds/refs/heads/main/openapi/hotelbeds-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Hotelbeds Authentication
name_suffix: Authentication
oauth_flows: []
overview: Hotelbeds secures its APIs with apiKey across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Hotelbeds
provider_slug: hotelbeds
scheme_count: 2
schemes:
- description: Your APItude API key, issued per API suite (Hotel, Activities, Transfers).
  in: header
  name: ApiKeyAuth
  parameter: Api-key
  sources:
  - openapi/hotelbeds-openapi.yml
  type: apiKey
- description: SHA256 hash, in hexadecimal, of the concatenation of the API key, the shared secret, and the current Unix timestamp in seconds.
  in: header
  name: SignatureAuth
  parameter: X-Signature
  sources:
  - openapi/hotelbeds-openapi.yml
  type: apiKey
slug: hotelbeds-authentication
source_filename: hotelbeds-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/hotelbeds-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: ApiKeyAuth\n  type: apiKey\n  in: header\n  parameter: Api-key\n  description: Your APItude API key, issued per API suite (Hotel, Activities, Transfers).\n  sources:\n  - openapi/hotelbeds-openapi.yml\n- name: SignatureAuth\n  type: apiKey\n  in: header\n  parameter: X-Signature\n  description: SHA256 hash, in hexadecimal, of the concatenation of the API key, the shared\n    secret, and the current Unix timestamp in seconds.\n  sources:\n  - openapi/hotelbeds-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/hotelbeds/refs/heads/main/authentication/hotelbeds-authentication.yml
summary_line: apiKey · 2 schemes
tags:
- Travel
- Hotels
- Bedbank
- Accommodation
- Booking
---
