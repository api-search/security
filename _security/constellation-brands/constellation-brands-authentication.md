---
api_key_in:
- query
api_specs:
- filename: constellation-brands-openapi.yml
  format: yaml
  label: Product Items API
  slug: product
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/constellation-brands/refs/heads/main/openapi/constellation-brands-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Constellation Brands Authentication
name_suffix: Authentication
oauth_flows: []
overview: Constellation Brands secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Constellation Brands
provider_slug: constellation-brands
scheme_count: 1
schemes:
- in: query
  name: ApiKeyAuth
  parameter: apiKey
  sources:
  - openapi/constellation-brands-openapi.yml
  type: apiKey
slug: constellation-brands-authentication
source_filename: constellation-brands-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/constellation-brands-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - query\nschemes:\n- name: ApiKeyAuth\n  type: apiKey\n  in: query\n  parameter: apiKey\n  sources:\n  - openapi/constellation-brands-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/constellation-brands/refs/heads/main/authentication/constellation-brands-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Alcohol
- Beer
- Beverages
- Digital Assets
- Fortune 500
- Spirits
- Wine
---
