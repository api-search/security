---
api_key_in:
- header
api_specs:
- filename: merkle-science-kybb-openapi.yml
  format: yaml
  label: Merkle Science KYBB API
  slug: merkle-science-kybb-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/merkle-science/refs/heads/main/openapi/merkle-science-kybb-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: searched
name: Merkle Science Authentication
name_suffix: Authentication
oauth_flows: []
overview: Merkle Science secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Merkle Science
provider_slug: merkle-science
scheme_count: 1
schemes:
- in: header
  name: ApiKeyAuth
  parameter: x-api-key
  sources:
  - openapi/merkle-science-kybb-openapi.yml
  type: apiKey
slug: merkle-science-authentication
source_filename: merkle-science-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: searched\nsource: openapi/merkle-science-kybb-openapi.yml\ndocs: https://kybb.docs.merklescience.com/reference/authentication\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nnotes: >-\n  The KYBB API authenticates every request with an API key passed in the x-api-key\n  request header. All requests must use HTTPS; unencrypted HTTP calls and requests\n  missing the header are rejected. API keys are issued directly by Merkle Science\n  (there is no self-service key provisioning); contact support@merklescience.com to\n  obtain one. Separate keys apply per environment (sandbox vs production) and, in the\n  Compass product, per workspace.\nschemes:\n- name: ApiKeyAuth\n  type: apiKey\n  in: header\n  parameter: x-api-key\n  sources:\n  - openapi/merkle-science-kybb-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/merkle-science/refs/heads/main/authentication/merkle-science-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Company
- Blockchain Analytics
- Cryptocurrency
- Compliance
- AML
- KYC
- Risk
- Fraud Detection
- Due Diligence
- RegTech
---
