---
api_key_in:
- header
api_specs:
- filename: picker-openapi-original.json
  format: json
  label: Picker API
  slug: picker-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/picker/refs/heads/main/openapi/picker-openapi-original.json
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: searched
name: Picker Authentication
name_suffix: Authentication
oauth_flows: []
overview: Picker secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Picker
provider_slug: picker
scheme_count: 1
schemes:
- description: Per-store API Key issued from the Picker Dashboard (dashboard.pickerexpress.com, Account/Locales). Required on all API and plugin requests; requires the Pro Plan.
  in: header
  key_name: authorization
  name: apiKey
  obtain_key: https://dashboard.pickerexpress.com/
  sources:
  - openapi/picker-openapi-original.json
  type: apiKey
slug: picker-authentication
source_filename: picker-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: searched\nsource: https://www.pickerexpress.com/en/developers/api-delivery-documentation\ndocs: https://app.theneo.io/pickerexpress/picker-api-suite/autenticacion\nsummary:\n  types: [apiKey]\n  api_key_in: [header]\n  api_key_name: authorization\n  notes: >-\n    The published Picker Production Swagger 2.0 declares no securityDefinitions,\n    but every request carries an `authorization` HTTP header. Per the developer\n    documentation, merchants authenticate with a per-store API Key obtained from\n    the Picker Dashboard (Account / Locales section); the Pro Plan must be active\n    to use the API and plugins. The key is passed in the `authorization` request\n    header.\nschemes:\n- name: apiKey\n  type: apiKey\n  in: header\n  key_name: authorization\n  description: >-\n    Per-store API Key issued from the Picker Dashboard (dashboard.pickerexpress.com,\n    Account/Locales). Required on all API and plugin requests; requires the Pro Plan.\n\
  \  obtain_key: https://dashboard.pickerexpress.com/\n  sources: [openapi/picker-openapi-original.json]\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/picker/refs/heads/main/authentication/picker-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Company
- Logistics
- Delivery
- Last Mile
- Courier
- E-commerce
- Shipping
- Tracking
- Latin America
- Fleet Management
---
