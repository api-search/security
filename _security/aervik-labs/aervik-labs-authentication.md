---
anonymous_access: false
api_key_in:
- header
api_specs:
- filename: aervik-labs-parse-api-openapi.yml
  format: yaml
  label: Aervik Labs Parse API
  slug: aervik-labs-parse-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aervik-labs/refs/heads/main/openapi/aervik-labs-parse-api-openapi.yml
- filename: aervik-labs-requirements-api-openapi.yml
  format: yaml
  label: Aervik Labs Requirements API
  slug: aervik-labs-requirements-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aervik-labs/refs/heads/main/openapi/aervik-labs-requirements-api-openapi.yml
- filename: aervik-labs-verify-api-openapi.yml
  format: yaml
  label: Aervik Labs Verify API
  slug: aervik-labs-verify-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aervik-labs/refs/heads/main/openapi/aervik-labs-verify-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Aervik Labs Authentication
name_suffix: Authentication
oauth_flows: []
overview: Aervik Labs secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Aervik Labs
provider_slug: aervik-labs
scheme_count: 1
schemes:
- description: Your RapidAPI application key.
  in: header
  name: RapidApiKey
  parameter: X-RapidAPI-Key
  sources:
  - openapi/aervik-labs-coi-verification.json
  type: apiKey
slug: aervik-labs-authentication
source_filename: aervik-labs-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-09-14'\nmethod: searched\nsource: openapi/aervik-labs-coi-verification.json ; https://aerviklabs.com/apis/coi-verification/\ndocs: https://aerviklabs.com/apis/coi-verification/\ndocs_note: >-\n  Docs confirm RapidAPI header auth: X-RapidAPI-Key (the application key) plus\n  X-RapidAPI-Host set to\n  certificate-of-insurance-verification-compliance-check-api.p.rapidapi.com.\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: RapidApiKey\n  type: apiKey\n  in: header\n  parameter: X-RapidAPI-Key\n  description: Your RapidAPI application key.\n  sources:\n  - openapi/aervik-labs-coi-verification.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/aervik-labs/refs/heads/main/authentication/aervik-labs-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Insurance
- Compliance
- Verification
- Insurtech
- Certificate of Insurance
- ACORD 25
- Document Intelligence
- RapidAPI
---
