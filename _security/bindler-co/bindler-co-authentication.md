---
anonymous_access: false
api_key_in:
- header
- query
api_specs:
- filename: bindler-co-ai-act-classify-api-openapi.yml
  format: yaml
  label: Bindler Ai Act Classify API
  slug: bindler-co-ai-act-classify-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/bindler-co/openapi/bindler-co-ai-act-classify-api-openapi.yml
- filename: bindler-co-cbam-cost-api-openapi.yml
  format: yaml
  label: Bindler Cbam Cost API
  slug: bindler-co-cbam-cost-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/bindler-co/openapi/bindler-co-cbam-cost-api-openapi.yml
- filename: bindler-co-uae-corporate-tax-api-openapi.yml
  format: yaml
  label: Bindler Uae Corporate Tax API
  slug: bindler-co-uae-corporate-tax-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/bindler-co/openapi/bindler-co-uae-corporate-tax-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
mechanism_count: 2
method: derived
name: Bindler Authentication
name_suffix: Authentication
oauth_flows: []
overview: Bindler secures its APIs with apiKey across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Bindler
provider_slug: bindler-co
scheme_count: 2
schemes:
- description: Gumroad licence key for the product bindler-api, sent in the x-api-key header. Keys that do not match the four-group licence pattern are ignored and the call falls through to the free tier.
  in: header
  name: ApiKey
  parameter: x-api-key
  sources:
  - openapi/bindler-co-openapi.json
  type: apiKey
- description: The same Gumroad licence key passed as a query parameter instead of the header, accepted by every endpoint.
  in: query
  name: ApiKeyQuery
  parameter: key
  sources:
  - openapi/bindler-co-openapi.json
  type: apiKey
slug: bindler-co-authentication
source_filename: bindler-co-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-02'\nmethod: derived\nsource: openapi/bindler-co-openapi.json\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\n  - query\nschemes:\n- name: ApiKey\n  type: apiKey\n  in: header\n  parameter: x-api-key\n  description: Gumroad licence key for the product bindler-api, sent in the x-api-key header.\n    Keys that do not match the four-group licence pattern are ignored and the call falls through\n    to the free tier.\n  sources:\n  - openapi/bindler-co-openapi.json\n- name: ApiKeyQuery\n  type: apiKey\n  in: query\n  parameter: key\n  description: The same Gumroad licence key passed as a query parameter instead of the header,\n    accepted by every endpoint.\n  sources:\n  - openapi/bindler-co-openapi.json\n"
source_yaml_url: https://artifacts.apis.io/bindler-co/authentication/bindler-co-authentication.yml
summary_line: apiKey · 2 schemes
tags:
- Company
- Data
- Finance
- Regulations
- Tools
---
