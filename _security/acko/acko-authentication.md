---
api_key_in:
- header
api_specs:
- filename: acko-apisetu-openapi-original.json
  format: json
  label: Acko General Insurance (API Setu / DigiLocker)
  slug: acko-general-insurance-api-setu-digilocker
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/acko/refs/heads/main/openapi/acko-apisetu-openapi-original.json
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Acko Authentication
name_suffix: Authentication
oauth_flows: []
overview: Acko secures its APIs with apiKey across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Acko
provider_slug: acko
scheme_count: 2
schemes:
- in: header
  name: apiKey
  parameter: X-APISETU-APIKEY
  sources:
  - openapi/acko-apisetu-openapi-original.json
  type: apiKey
- in: header
  name: clientId
  parameter: X-APISETU-CLIENTID
  sources:
  - openapi/acko-apisetu-openapi-original.json
  type: apiKey
slug: acko-authentication
source_filename: acko-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: derived\nsource: openapi/acko-apisetu-openapi-original.json\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: apiKey\n  type: apiKey\n  in: header\n  parameter: X-APISETU-APIKEY\n  sources:\n  - openapi/acko-apisetu-openapi-original.json\n- name: clientId\n  type: apiKey\n  in: header\n  parameter: X-APISETU-CLIENTID\n  sources:\n  - openapi/acko-apisetu-openapi-original.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/acko/refs/heads/main/authentication/acko-authentication.yml
summary_line: apiKey · 2 schemes
tags:
- Company
- Consumer
- Insurance
- InsurTech
- Financial Services
- Digital Insurance
- India
- Embedded Insurance
---
