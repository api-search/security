---
api_key_in:
- header
api_specs:
- filename: recreation-gov-activities-api-openapi.yml
  format: yaml
  label: Recreation.gov Activities API
  slug: recreation-gov-activities-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/recreation-gov/refs/heads/main/openapi/recreation-gov-activities-api-openapi.yml
- filename: recreation-gov-campsites-api-openapi.yml
  format: yaml
  label: Recreation.gov Campsites API
  slug: recreation-gov-campsites-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/recreation-gov/refs/heads/main/openapi/recreation-gov-campsites-api-openapi.yml
- filename: recreation-gov-events-api-openapi.yml
  format: yaml
  label: Recreation.gov Events API
  slug: recreation-gov-events-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/recreation-gov/refs/heads/main/openapi/recreation-gov-events-api-openapi.yml
- filename: recreation-gov-facilities-api-openapi.yml
  format: yaml
  label: Recreation.gov Facilities API
  slug: recreation-gov-facilities-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/recreation-gov/refs/heads/main/openapi/recreation-gov-facilities-api-openapi.yml
- filename: recreation-gov-links-api-openapi.yml
  format: yaml
  label: Recreation.gov Links API
  slug: recreation-gov-links-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/recreation-gov/refs/heads/main/openapi/recreation-gov-links-api-openapi.yml
- filename: recreation-gov-media-api-openapi.yml
  format: yaml
  label: Recreation.gov Media API
  slug: recreation-gov-media-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/recreation-gov/refs/heads/main/openapi/recreation-gov-media-api-openapi.yml
- filename: recreation-gov-organizations-api-openapi.yml
  format: yaml
  label: Recreation.gov Organizations API
  slug: recreation-gov-organizations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/recreation-gov/refs/heads/main/openapi/recreation-gov-organizations-api-openapi.yml
- filename: recreation-gov-permitentrances-api-openapi.yml
  format: yaml
  label: Recreation.gov Permitentrances API
  slug: recreation-gov-permitentrances-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/recreation-gov/refs/heads/main/openapi/recreation-gov-permitentrances-api-openapi.yml
- filename: recreation-gov-recareas-api-openapi.yml
  format: yaml
  label: Recreation.gov Recareas API
  slug: recreation-gov-recareas-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/recreation-gov/refs/heads/main/openapi/recreation-gov-recareas-api-openapi.yml
- filename: recreation-gov-tours-api-openapi.yml
  format: yaml
  label: Recreation.gov Tours API
  slug: recreation-gov-tours-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/recreation-gov/refs/heads/main/openapi/recreation-gov-tours-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Recreation Gov Authentication
name_suffix: Authentication
oauth_flows: []
overview: Recreation.gov secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Recreation.gov
provider_slug: recreation-gov
scheme_count: 1
schemes:
- in: header
  name: apiKey
  parameter: apikey
  sources:
  - openapi/recreation-gov-openapi.yml
  type: apiKey
slug: recreation-gov-authentication
source_filename: recreation-gov-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/recreation-gov-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: apiKey\n  type: apiKey\n  in: header\n  parameter: apikey\n  sources:\n  - openapi/recreation-gov-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/recreation-gov/refs/heads/main/authentication/recreation-gov-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Recreation
- Federal
- Camping
- Outdoors
- Public Lands
---
