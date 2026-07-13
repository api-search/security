---
api_key_in: []
api_specs:
- filename: uplisting-openapi.yml
  format: yaml
  label: Uplisting Bookings API
  slug: uplisting-bookings-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/uplisting/refs/heads/main/openapi/uplisting-openapi.yml
- filename: uplisting-openapi.yml
  format: yaml
  label: Uplisting Properties API
  slug: uplisting-properties-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/uplisting/refs/heads/main/openapi/uplisting-openapi.yml
- filename: uplisting-openapi.yml
  format: yaml
  label: Uplisting Availability API
  slug: uplisting-availability-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/uplisting/refs/heads/main/openapi/uplisting-openapi.yml
- filename: uplisting-openapi.yml
  format: yaml
  label: Uplisting Calendar API
  slug: uplisting-calendar-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/uplisting/refs/heads/main/openapi/uplisting-openapi.yml
- filename: uplisting-openapi.yml
  format: yaml
  label: Uplisting Rates API
  slug: uplisting-rates-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/uplisting/refs/heads/main/openapi/uplisting-openapi.yml
- filename: uplisting-openapi.yml
  format: yaml
  label: Uplisting Guests API
  slug: uplisting-guests-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/uplisting/refs/heads/main/openapi/uplisting-openapi.yml
- filename: uplisting-openapi.yml
  format: yaml
  label: Uplisting Messages API
  slug: uplisting-messages-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/uplisting/refs/heads/main/openapi/uplisting-openapi.yml
- filename: uplisting-openapi.yml
  format: yaml
  label: Uplisting Webhooks API
  slug: uplisting-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/uplisting/refs/heads/main/openapi/uplisting-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Uplisting Authentication
name_suffix: Authentication
oauth_flows: []
overview: Uplisting secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Uplisting
provider_slug: uplisting
scheme_count: 1
schemes:
- description: 'HTTP Basic auth. Send `Authorization: Basic <base64(api_key)>`, where api_key is generated on the Uplisting Connect page. V2 endpoints also require a Client ID partner identifier.'
  name: basicAuth
  scheme: basic
  sources:
  - openapi/uplisting-openapi.yml
  type: http
slug: uplisting-authentication
source_filename: uplisting-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/uplisting-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: basicAuth\n  type: http\n  scheme: basic\n  description: 'HTTP Basic auth. Send `Authorization: Basic <base64(api_key)>`, where api_key\n    is generated on the Uplisting Connect page. V2 endpoints also require a Client ID partner\n    identifier.'\n  sources:\n  - openapi/uplisting-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/uplisting/refs/heads/main/authentication/uplisting-authentication.yml
summary_line: http · 1 scheme
tags:
- Vacation Rental
- Short-Term Rental
- Channel Manager
- Property Management
- Bookings
- Hospitality
---
