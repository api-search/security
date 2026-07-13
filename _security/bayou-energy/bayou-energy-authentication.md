---
api_key_in: []
api_specs:
- filename: bayou-energy-openapi.yml
  format: yaml
  label: Bayou Energy Customers API
  slug: customers
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bayou-energy/refs/heads/main/openapi/bayou-energy-openapi.yml
- filename: bayou-energy-openapi.yml
  format: yaml
  label: Bayou Energy Bills API
  slug: bills
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bayou-energy/refs/heads/main/openapi/bayou-energy-openapi.yml
- filename: bayou-energy-openapi.yml
  format: yaml
  label: Bayou Energy Intervals API
  slug: intervals
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bayou-energy/refs/heads/main/openapi/bayou-energy-openapi.yml
- filename: bayou-energy-openapi.yml
  format: yaml
  label: Bayou Energy Meters API
  slug: meters
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bayou-energy/refs/heads/main/openapi/bayou-energy-openapi.yml
- filename: bayou-energy-openapi.yml
  format: yaml
  label: Bayou Energy Webhooks API
  slug: webhooks
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bayou-energy/refs/heads/main/openapi/bayou-energy-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Bayou Energy Authentication
name_suffix: Authentication
oauth_flows: []
overview: Bayou Energy secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Bayou Energy
provider_slug: bayou-energy
scheme_count: 1
schemes:
- description: HTTP Basic authentication. Use your API key as the username and leave the password empty.
  name: basicAuth
  scheme: basic
  sources:
  - openapi/bayou-energy-openapi.yml
  type: http
slug: bayou-energy-authentication
source_filename: bayou-energy-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/bayou-energy-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: basicAuth\n  type: http\n  scheme: basic\n  description: HTTP Basic authentication. Use your API key as the username and leave the password\n    empty.\n  sources:\n  - openapi/bayou-energy-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/bayou-energy/refs/heads/main/authentication/bayou-energy-authentication.yml
summary_line: http · 1 scheme
tags:
- Utility Data
- Energy
- Utility Bills
- Interval Data
- Metering
---
