---
api_key_in:
- header
api_specs:
- filename: postman.yaml
  format: yaml
  label: Proton API
  slug: proton-api
  spec_type: Postman
  url: https://api.proton.ai/
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: searched
name: Proton Authentication
name_suffix: Authentication
oauth_flows: []
overview: Proton.ai secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Proton.ai
provider_slug: proton
scheme_count: 1
schemes:
- in: header
  name: apiKey
  sources:
  - https://api.proton.ai/
  static: true
  type: apiKey
slug: proton-authentication
source_filename: proton-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: searched\nsource: https://api.proton.ai/\ndocs: https://api.proton.ai/\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\n  oauth2_flows: []\n  notes: >-\n    Proton.ai documents a static API key passed in the request header. Per the published\n    documentation the key is issued at the start of an integration and does not need to be\n    dynamically generated or refreshed. The exact header parameter name is not disclosed in\n    the public Postman documentation, so it is not recorded here to avoid fabrication.\nschemes:\n- name: apiKey\n  type: apiKey\n  in: header\n  static: true\n  sources:\n  - https://api.proton.ai/\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/proton/refs/heads/main/authentication/proton-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Company
- Artificial Intelligence
- Distribution
- Wholesale
- B2B
- Sales
- Recommendations
- CRM
- e-Commerce
---
