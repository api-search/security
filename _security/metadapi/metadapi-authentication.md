---
anonymous_access: false
api_key_in:
- header
api_specs:
- filename: metadapi-zipc-api-openapi.yml
  format: yaml
  label: Metadapi Zipc API
  slug: metadapi-zipc-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/metadapi/openapi/metadapi-zipc-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: derived
name: Metadapi Authentication
name_suffix: Authentication
oauth_flows: []
overview: Metadapi secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Metadapi
provider_slug: metadapi
scheme_count: 1
schemes:
- description: API Key provided by the metadapi subscription.
  in: header
  name: subscription-key
  parameter: Ocp-Apim-Subscription-Key
  sources:
  - openapi/metadapi-zipcode-openapi.json
  type: apiKey
slug: metadapi-authentication
source_filename: metadapi-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-10-20'\nmethod: derived\nsource: openapi/metadapi-zipcode-openapi.json\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: subscription-key\n  type: apiKey\n  in: header\n  parameter: Ocp-Apim-Subscription-Key\n  description: API Key provided by the metadapi subscription.\n  sources:\n  - openapi/metadapi-zipcode-openapi.json\n"
source_yaml_url: https://artifacts.apis.io/metadapi/authentication/metadapi-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Company
- Data
- Reference
- JSON
---
