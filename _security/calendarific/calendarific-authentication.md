---
api_key_in:
- query
api_specs:
- filename: calendarific-countries-api-openapi.yml
  format: yaml
  label: Calendarific Countries API
  slug: calendarific-countries-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/calendarific/refs/heads/main/openapi/calendarific-countries-api-openapi.yml
- filename: calendarific-holidays-api-openapi.yml
  format: yaml
  label: Calendarific Holidays API
  slug: calendarific-holidays-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/calendarific/refs/heads/main/openapi/calendarific-holidays-api-openapi.yml
- filename: calendarific-languages-api-openapi.yml
  format: yaml
  label: Calendarific Languages API
  slug: calendarific-languages-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/calendarific/refs/heads/main/openapi/calendarific-languages-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Calendarific Authentication
name_suffix: Authentication
oauth_flows: []
overview: Calendarific secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Calendarific
provider_slug: calendarific
scheme_count: 1
schemes:
- description: API key passed as a URL query parameter.
  in: query
  name: apiKey
  parameter: api_key
  sources:
  - openapi/calendarific-openapi.yml
  type: apiKey
slug: calendarific-authentication
source_filename: calendarific-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/calendarific-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - query\nschemes:\n- name: apiKey\n  type: apiKey\n  in: query\n  parameter: api_key\n  description: API key passed as a URL query parameter.\n  sources:\n  - openapi/calendarific-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/calendarific/refs/heads/main/authentication/calendarific-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Calendar
- Public APIs
- Holidays
- Worldwide
- Localization
---
