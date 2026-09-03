---
api_key_in:
- header
api_specs:
- filename: taylor-morrison-home-communities-api-openapi.yml
  format: yaml
  label: taylor-morrison-home Communities API
  slug: taylor-morrison-home-communities-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/taylor-morrison-home/refs/heads/main/openapi/taylor-morrison-home-communities-api-openapi.yml
- filename: taylor-morrison-home-design-api-openapi.yml
  format: yaml
  label: taylor-morrison-home Design API
  slug: taylor-morrison-home-design-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/taylor-morrison-home/refs/heads/main/openapi/taylor-morrison-home-design-api-openapi.yml
- filename: taylor-morrison-home-floor-plans-api-openapi.yml
  format: yaml
  label: taylor-morrison-home Floor Plans API
  slug: taylor-morrison-home-floor-plans-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/taylor-morrison-home/refs/heads/main/openapi/taylor-morrison-home-floor-plans-api-openapi.yml
- filename: taylor-morrison-home-homes-api-openapi.yml
  format: yaml
  label: taylor-morrison-home Homes API
  slug: taylor-morrison-home-homes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/taylor-morrison-home/refs/heads/main/openapi/taylor-morrison-home-homes-api-openapi.yml
- filename: taylor-morrison-home-lots-api-openapi.yml
  format: yaml
  label: taylor-morrison-home Lots API
  slug: taylor-morrison-home-lots-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/taylor-morrison-home/refs/heads/main/openapi/taylor-morrison-home-lots-api-openapi.yml
- filename: taylor-morrison-home-reservations-api-openapi.yml
  format: yaml
  label: taylor-morrison-home Reservations API
  slug: taylor-morrison-home-reservations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/taylor-morrison-home/refs/heads/main/openapi/taylor-morrison-home-reservations-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Taylor Morrison Home Authentication
name_suffix: Authentication
oauth_flows: []
overview: Taylor Morrison Home secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Taylor Morrison Home
provider_slug: taylor-morrison-home
scheme_count: 1
schemes:
- in: header
  name: apiKeyAuth
  parameter: X-API-Key
  sources:
  - openapi/taylor-morrison-home-search-openapi.yml
  type: apiKey
slug: taylor-morrison-home-authentication
source_filename: taylor-morrison-home-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/taylor-morrison-home-search-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: apiKeyAuth\n  type: apiKey\n  in: header\n  parameter: X-API-Key\n  sources:\n  - openapi/taylor-morrison-home-search-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/taylor-morrison-home/refs/heads/main/authentication/taylor-morrison-home-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Homebuilding
- Real-Estate
- Fortune 1000
- New Homes
- Communities
- Mortgage
---
