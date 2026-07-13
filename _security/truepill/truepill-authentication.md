---
api_key_in:
- header
api_specs:
- filename: truepill-openapi.yml
  format: yaml
  label: Truepill Patients API
  slug: truepill-patients-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/truepill/refs/heads/main/openapi/truepill-openapi.yml
- filename: truepill-openapi.yml
  format: yaml
  label: Truepill Prescriptions & Orders API
  slug: truepill-prescriptions-orders-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/truepill/refs/heads/main/openapi/truepill-openapi.yml
- filename: truepill-openapi.yml
  format: yaml
  label: Truepill Medications & Insurance API
  slug: truepill-medications-insurance-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/truepill/refs/heads/main/openapi/truepill-openapi.yml
- filename: truepill-openapi.yml
  format: yaml
  label: Truepill Shipments & Fulfillment API
  slug: truepill-shipments-fulfillment-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/truepill/refs/heads/main/openapi/truepill-openapi.yml
- filename: truepill-openapi.yml
  format: yaml
  label: Truepill Webhooks API
  slug: truepill-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/truepill/refs/heads/main/openapi/truepill-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Truepill Authentication
name_suffix: Authentication
oauth_flows: []
overview: Truepill secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Truepill
provider_slug: truepill
scheme_count: 1
schemes:
- description: 'API key passed as `Authorization: ApiKey <YOUR_API_KEY>`. Separate keys are issued for the sandbox and production environments.'
  in: header
  name: ApiKeyAuth
  parameter: Authorization
  sources:
  - openapi/truepill-openapi.yml
  type: apiKey
slug: truepill-authentication
source_filename: truepill-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/truepill-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: ApiKeyAuth\n  type: apiKey\n  in: header\n  parameter: Authorization\n  description: 'API key passed as `Authorization: ApiKey <YOUR_API_KEY>`. Separate keys are\n    issued for the sandbox and production environments.'\n  sources:\n  - openapi/truepill-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/truepill/refs/heads/main/authentication/truepill-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Pharmacy
- Healthcare
- Prescription Fulfillment
- Telehealth
- Diagnostics
- Insurance
---
