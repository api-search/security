---
api_key_in:
- header
api_specs:
- filename: nuitee-openapi.yml
  format: yaml
  label: LiteAPI Hotel Data API
  slug: hotel-data
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nuitee/refs/heads/main/openapi/nuitee-openapi.yml
- filename: nuitee-openapi.yml
  format: yaml
  label: LiteAPI Rates Search API
  slug: rates-search
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nuitee/refs/heads/main/openapi/nuitee-openapi.yml
- filename: nuitee-openapi.yml
  format: yaml
  label: LiteAPI Booking API
  slug: booking
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nuitee/refs/heads/main/openapi/nuitee-openapi.yml
- filename: nuitee-openapi.yml
  format: yaml
  label: LiteAPI Loyalty and Vouchers API
  slug: loyalty-vouchers
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nuitee/refs/heads/main/openapi/nuitee-openapi.yml
- filename: nuitee-openapi.yml
  format: yaml
  label: LiteAPI Webhooks
  slug: webhooks
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nuitee/refs/heads/main/openapi/nuitee-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Nuitee Authentication
name_suffix: Authentication
oauth_flows: []
overview: Nuitée (LiteAPI) secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Nuitée (LiteAPI)
provider_slug: nuitee
scheme_count: 1
schemes:
- description: LiteAPI key passed in the X-API-Key request header. A free sandbox key is available; live keys are issued from the LiteAPI dashboard.
  in: header
  name: ApiKeyAuth
  parameter: X-API-Key
  sources:
  - openapi/nuitee-openapi.yml
  type: apiKey
slug: nuitee-authentication
source_filename: nuitee-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/nuitee-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: ApiKeyAuth\n  type: apiKey\n  in: header\n  parameter: X-API-Key\n  description: LiteAPI key passed in the X-API-Key request header. A free sandbox key is available;\n    live keys are issued from the LiteAPI dashboard.\n  sources:\n  - openapi/nuitee-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/nuitee/refs/heads/main/authentication/nuitee-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Travel
- Hotels
- Booking
- Distribution
- Hospitality
---
