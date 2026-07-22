---
api_key_in:
- header
api_specs:
- filename: onsi-openapi-original.json
  format: json
  label: Onsi Partner API
  slug: onsi-partner-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/onsi/refs/heads/main/openapi/onsi-openapi-original.json
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: searched
name: Onsi Authentication
name_suffix: Authentication
oauth_flows: []
overview: Onsi secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Onsi
provider_slug: onsi
scheme_count: 1
schemes:
- docs: https://docs.onsi.com/api-reference/introduction
  in: header
  name: apiKey
  parameter: x-api-key
  sources:
  - openapi/onsi-openapi-original.json
  type: apiKey
slug: onsi-authentication
source_filename: onsi-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: searched\nsource: openapi/onsi-openapi-original.json\ndocs: https://docs.onsi.com/api-reference/introduction\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\n  key_provisioning: Request an API key from the Onsi team; a distinct key is issued per environment (production vs sandbox api.onsi.dev).\nschemes:\n- name: apiKey\n  type: apiKey\n  in: header\n  parameter: x-api-key\n  docs: https://docs.onsi.com/api-reference/introduction\n  sources:\n  - openapi/onsi-openapi-original.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/onsi/refs/heads/main/authentication/onsi-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Company
- Benefits
- Earned Wage Access
- On-Demand Pay
- Payroll
- Fintech
- Insurance
- Workforce
- HR
- Health
---
