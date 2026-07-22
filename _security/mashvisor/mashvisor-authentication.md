---
api_key_in:
- header
api_specs:
- filename: mashvisor-openapi.yml
  format: yaml
  label: Mashvisor Data API
  slug: mashvisor-data-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mashvisor/refs/heads/main/openapi/mashvisor-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Mashvisor Authentication
name_suffix: Authentication
oauth_flows: []
overview: Mashvisor secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Mashvisor
provider_slug: mashvisor
scheme_count: 1
schemes:
- description: Include your secret API key in the `x-api-key` header on every request. Obtain a key by registering for a developer account at mashvisor.com.
  in: header
  name: apiKey
  parameter: x-api-key
  sources:
  - openapi/mashvisor-openapi.yml
  type: apiKey
slug: mashvisor-authentication
source_filename: mashvisor-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: derived\nsource: openapi/mashvisor-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: apiKey\n  type: apiKey\n  in: header\n  parameter: x-api-key\n  description: Include your secret API key in the `x-api-key` header on every request. Obtain\n    a key by registering for a developer account at mashvisor.com.\n  sources:\n  - openapi/mashvisor-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/mashvisor/refs/heads/main/authentication/mashvisor-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Company
- Real Estate
- Property Data
- Analytics
- Rental
- Airbnb
- Investment
- MLS
- Housing
---
