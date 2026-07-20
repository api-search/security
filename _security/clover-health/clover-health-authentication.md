---
api_key_in:
- cookie
api_specs:
- filename: clover-health-fhir-openapi-original.yml
  format: yaml
  label: Clover Health FHIR API (Formulary & Provider Directory)
  slug: clover-health-fhir-api-formulary-provider-directory
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/clover-health/refs/heads/main/openapi/clover-health-fhir-openapi-original.yml
auth_types:
- apiKey
- http
description: ''
kind: authentication
layout: security
method: derived
name: Clover Health Authentication
name_suffix: Authentication
oauth_flows: []
overview: Clover Health secures its APIs with apiKey and http across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Clover Health
provider_slug: clover-health
scheme_count: 2
schemes:
- name: basicAuth
  scheme: basic
  sources:
  - openapi/clover-health-fhir-openapi-original.yml
  type: http
- in: cookie
  name: cookieAuth
  parameter: sessionid
  sources:
  - openapi/clover-health-fhir-openapi-original.yml
  type: apiKey
slug: clover-health-authentication
source_filename: clover-health-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: derived\nsource: openapi/clover-health-fhir-openapi-original.yml\nsummary:\n  types:\n  - apiKey\n  - http\n  api_key_in:\n  - cookie\nschemes:\n- name: basicAuth\n  type: http\n  scheme: basic\n  sources:\n  - openapi/clover-health-fhir-openapi-original.yml\n- name: cookieAuth\n  type: apiKey\n  in: cookie\n  parameter: sessionid\n  sources:\n  - openapi/clover-health-fhir-openapi-original.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/clover-health/refs/heads/main/authentication/clover-health-authentication.yml
summary_line: apiKey/http · 2 schemes
tags:
- Company
- Healthcare
- Health Insurance
- Medicare Advantage
- FHIR
- Interoperability
- Provider Directory
- Formulary
- Patient Access
- Payer
---
