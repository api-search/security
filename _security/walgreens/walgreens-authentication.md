---
api_key_in:
- query
api_specs:
- filename: walgreens-appointments-api-openapi.yml
  format: yaml
  label: Walgreens Appointments API
  slug: walgreens-appointments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/walgreens/refs/heads/main/openapi/walgreens-appointments-api-openapi.yml
- filename: walgreens-eligibility-api-openapi.yml
  format: yaml
  label: Walgreens Eligibility API
  slug: walgreens-eligibility-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/walgreens/refs/heads/main/openapi/walgreens-eligibility-api-openapi.yml
- filename: walgreens-patients-api-openapi.yml
  format: yaml
  label: Walgreens Patients API
  slug: walgreens-patients-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/walgreens/refs/heads/main/openapi/walgreens-patients-api-openapi.yml
- filename: walgreens-refills-api-openapi.yml
  format: yaml
  label: Walgreens Refills API
  slug: walgreens-refills-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/walgreens/refs/heads/main/openapi/walgreens-refills-api-openapi.yml
- filename: walgreens-stores-api-openapi.yml
  format: yaml
  label: Walgreens Stores API
  slug: walgreens-stores-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/walgreens/refs/heads/main/openapi/walgreens-stores-api-openapi.yml
- filename: walgreens-transfers-api-openapi.yml
  format: yaml
  label: Walgreens Transfers API
  slug: walgreens-transfers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/walgreens/refs/heads/main/openapi/walgreens-transfers-api-openapi.yml
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
