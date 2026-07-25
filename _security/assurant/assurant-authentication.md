---
api_key_in:
- header
api_specs:
- filename: assurant-claims-api-openapi.yml
  format: yaml
  label: Assurant Claims API
  slug: assurant-claims-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/assurant/refs/heads/main/openapi/assurant-claims-api-openapi.yml
- filename: assurant-enrollments-api-openapi.yml
  format: yaml
  label: Assurant Enrollments API
  slug: assurant-enrollments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/assurant/refs/heads/main/openapi/assurant-enrollments-api-openapi.yml
- filename: assurant-policies-api-openapi.yml
  format: yaml
  label: Assurant Policies API
  slug: assurant-policies-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/assurant/refs/heads/main/openapi/assurant-policies-api-openapi.yml
- filename: assurant-products-api-openapi.yml
  format: yaml
  label: Assurant Products API
  slug: assurant-products-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/assurant/refs/heads/main/openapi/assurant-products-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Assurant Authentication
name_suffix: Authentication
oauth_flows: []
overview: Assurant secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Assurant
provider_slug: assurant
scheme_count: 1
schemes:
- in: header
  name: apiKeyAuth
  parameter: X-API-Key
  sources:
  - openapi/assurant-apex-insurance-api-openapi.yml
  type: apiKey
slug: assurant-authentication
source_filename: assurant-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/assurant-apex-insurance-api-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: apiKeyAuth\n  type: apiKey\n  in: header\n  parameter: X-API-Key\n  sources:\n  - openapi/assurant-apex-insurance-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/assurant/refs/heads/main/authentication/assurant-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Insurance
- Device Protection
- Embedded Insurance
- Housing
- Claims
- Fortune 500
---
