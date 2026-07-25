---
api_key_in:
- header
api_specs:
- filename: nuitee-booking-api-openapi.yml
  format: yaml
  label: Nuitée (LiteAPI) Booking API
  slug: nuitee-booking-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nuitee/refs/heads/main/openapi/nuitee-booking-api-openapi.yml
- filename: nuitee-hotel-data-api-openapi.yml
  format: yaml
  label: Nuitée (LiteAPI) Hotel Data API
  slug: nuitee-hotel-data-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nuitee/refs/heads/main/openapi/nuitee-hotel-data-api-openapi.yml
- filename: nuitee-loyalty-api-openapi.yml
  format: yaml
  label: Nuitée (LiteAPI) Loyalty API
  slug: nuitee-loyalty-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nuitee/refs/heads/main/openapi/nuitee-loyalty-api-openapi.yml
- filename: nuitee-rates-api-openapi.yml
  format: yaml
  label: Nuitée (LiteAPI) Rates API
  slug: nuitee-rates-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nuitee/refs/heads/main/openapi/nuitee-rates-api-openapi.yml
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
