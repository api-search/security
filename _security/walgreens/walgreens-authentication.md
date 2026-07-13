---
api_key_in:
- query
api_specs:
- filename: walgreens-store-locator-openapi.yml
  format: yaml
  label: Walgreens Store Locator API
  slug: walgreens-store-locator
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/walgreens/refs/heads/main/openapi/walgreens-store-locator-openapi.yml
- filename: walgreens-prescription-refill-openapi.yml
  format: yaml
  label: Walgreens Prescription Refill API
  slug: walgreens-prescription-refill
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/walgreens/refs/heads/main/openapi/walgreens-prescription-refill-openapi.yml
- filename: walgreens-vaccine-scheduling-openapi.yml
  format: yaml
  label: Walgreens Vaccine Scheduling API
  slug: walgreens-vaccine-scheduling
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/walgreens/refs/heads/main/openapi/walgreens-vaccine-scheduling-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Walgreens Authentication
name_suffix: Authentication
oauth_flows: []
overview: Walgreens secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Walgreens
provider_slug: walgreens
scheme_count: 1
schemes:
- description: API key obtained from Walgreens Developer Portal
  in: query
  name: apiKey
  parameter: apiKey
  sources:
  - openapi/walgreens-prescription-refill-openapi.yml
  - openapi/walgreens-store-locator-openapi.yml
  - openapi/walgreens-vaccine-scheduling-openapi.yml
  type: apiKey
slug: walgreens-authentication
source_filename: walgreens-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/walgreens-prescription-refill-openapi.yml, openapi/walgreens-store-locator-openapi.yml,\n  openapi/walgreens-vaccine-scheduling-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - query\nschemes:\n- name: apiKey\n  type: apiKey\n  in: query\n  parameter: apiKey\n  description: API key obtained from Walgreens Developer Portal\n  sources:\n  - openapi/walgreens-prescription-refill-openapi.yml\n  - openapi/walgreens-store-locator-openapi.yml\n  - openapi/walgreens-vaccine-scheduling-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/walgreens/refs/heads/main/authentication/walgreens-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Pharmacy
- Healthcare
- Retail
- Prescriptions
- Vaccines
- Fortune 100
---
