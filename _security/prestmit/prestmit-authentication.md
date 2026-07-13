---
api_key_in:
- header
api_specs:
- filename: prestmit-openapi.yml
  format: yaml
  label: Prestmit Partner API
  slug: prestmit-partner-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/prestmit/refs/heads/main/openapi/prestmit-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Prestmit Authentication
name_suffix: Authentication
oauth_flows: []
overview: Prestmit secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Prestmit
provider_slug: prestmit
scheme_count: 1
schemes:
- description: 'Prestmit Partner API key issued from the developer dashboard. Optional

    IP whitelisting can be enabled per key.'
  in: header
  name: apiKey
  parameter: x-api-key
  sources:
  - openapi/prestmit-openapi.yml
  type: apiKey
slug: prestmit-authentication
source_filename: prestmit-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/prestmit-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: apiKey\n  type: apiKey\n  in: header\n  parameter: x-api-key\n  description: |-\n    Prestmit Partner API key issued from the developer dashboard. Optional\n    IP whitelisting can be enabled per key.\n  sources:\n  - openapi/prestmit-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/prestmit/refs/heads/main/authentication/prestmit-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Bills
- Crypto
- Fintech
- Gift Cards
- Payments
---
