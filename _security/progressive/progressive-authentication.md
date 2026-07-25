---
api_key_in: []
api_specs:
- filename: progressive-certificates-api-openapi.yml
  format: yaml
  label: Progressive Certificates API
  slug: progressive-certificates-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/progressive/refs/heads/main/openapi/progressive-certificates-api-openapi.yml
- filename: progressive-drivers-api-openapi.yml
  format: yaml
  label: Progressive Drivers API
  slug: progressive-drivers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/progressive/refs/heads/main/openapi/progressive-drivers-api-openapi.yml
- filename: progressive-policies-api-openapi.yml
  format: yaml
  label: Progressive Policies API
  slug: progressive-policies-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/progressive/refs/heads/main/openapi/progressive-policies-api-openapi.yml
- filename: progressive-quotes-api-openapi.yml
  format: yaml
  label: Progressive Quotes API
  slug: progressive-quotes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/progressive/refs/heads/main/openapi/progressive-quotes-api-openapi.yml
- filename: progressive-vehicles-api-openapi.yml
  format: yaml
  label: Progressive Vehicles API
  slug: progressive-vehicles-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/progressive/refs/heads/main/openapi/progressive-vehicles-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Progressive Authentication
name_suffix: Authentication
oauth_flows: []
overview: Progressive secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Progressive
provider_slug: progressive
scheme_count: 1
schemes:
- name: bearerAuth
  scheme: bearer
  sources:
  - openapi/progressive-auto-quote-api-openapi.yml
  - openapi/progressive-certificate-of-insurance-api-openapi.yml
  type: http
slug: progressive-authentication
source_filename: progressive-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/progressive-auto-quote-api-openapi.yml, openapi/progressive-certificate-of-insurance-api-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  sources:\n  - openapi/progressive-auto-quote-api-openapi.yml\n  - openapi/progressive-certificate-of-insurance-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/progressive/refs/heads/main/authentication/progressive-authentication.yml
summary_line: http · 1 scheme
tags:
- Auto Insurance
- Commercial Insurance
- Embedded Insurance
- Insurance
- Quoting
- Fortune 500
---
