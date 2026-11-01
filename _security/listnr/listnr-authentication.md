---
anonymous_access: false
api_key_in:
- header
api_specs:
- filename: listnr-agent-api-openapi.yml
  format: yaml
  label: Listnr Agent API
  slug: listnr-agent-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/listnr/openapi/listnr-agent-api-openapi.yml
- filename: listnr-billing-api-openapi.yml
  format: yaml
  label: Listnr Billing API
  slug: listnr-billing-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/listnr/openapi/listnr-billing-api-openapi.yml
- filename: listnr-catalog-api-openapi.yml
  format: yaml
  label: Listnr Catalog API
  slug: listnr-catalog-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/listnr/openapi/listnr-catalog-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: derived
name: Listnr Authentication
name_suffix: Authentication
oauth_flows: []
overview: Listnr secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Listnr
provider_slug: listnr
scheme_count: 1
schemes:
- description: Personal API key generated in the Listnr dashboard at voices.listnr.tech. Keep it server-side; never expose it in the browser or front-end code.
  in: header
  name: listnrToken
  parameter: x-listnr-token
  sources:
  - openapi/listnr-openapi.yml
  type: apiKey
slug: listnr-authentication
source_filename: listnr-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/listnr-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: listnrToken\n  type: apiKey\n  in: header\n  parameter: x-listnr-token\n  description: Personal API key generated in the Listnr dashboard at voices.listnr.tech. Keep\n    it server-side; never expose it in the browser or front-end code.\n  sources:\n  - openapi/listnr-openapi.yml\n"
source_yaml_url: https://artifacts.apis.io/listnr/authentication/listnr-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Artificial Intelligence
- Text-to-Speech
- Voice
- Speech Synthesis
- Audio
- Voiceover
---
