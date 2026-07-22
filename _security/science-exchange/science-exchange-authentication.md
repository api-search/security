---
api_key_in:
- query
api_specs:
- filename: science-exchange-providers-openapi.yml
  format: yaml
  label: Science Exchange Providers API
  slug: science-exchange-providers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/science-exchange/refs/heads/main/openapi/science-exchange-providers-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Science Exchange Authentication
name_suffix: Authentication
oauth_flows: []
overview: Science Exchange secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Science Exchange
provider_slug: science-exchange
scheme_count: 1
schemes:
- description: Provider API key passed as the access_token query parameter on every request.
  in: query
  name: access_token
  parameter: access_token
  sources:
  - openapi/science-exchange-providers-openapi.yml
  type: apiKey
slug: science-exchange-authentication
source_filename: science-exchange-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: derived\nsource: openapi/science-exchange-providers-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - query\nschemes:\n- name: access_token\n  type: apiKey\n  in: query\n  parameter: access_token\n  description: Provider API key passed as the access_token query parameter on every request.\n  sources:\n  - openapi/science-exchange-providers-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/science-exchange/refs/heads/main/authentication/science-exchange-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Company
- Life Sciences
- Research and Development
- Scientific Services
- Procurement
- Marketplace
- Supplier Management
- Biotech
- Pharmaceuticals
- API
---
