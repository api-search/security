---
api_key_in: []
api_specs:
- filename: opkit-benefits-api-openapi.yml
  format: yaml
  label: Opkit Benefits API
  slug: opkit-benefits-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/opkit/refs/heads/main/openapi/opkit-benefits-api-openapi.yml
- filename: opkit-eligibility-inquiries-api-openapi.yml
  format: yaml
  label: Opkit Eligibility Inquiries API
  slug: opkit-eligibility-inquiries-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/opkit/refs/heads/main/openapi/opkit-eligibility-inquiries-api-openapi.yml
- filename: opkit-patients-api-openapi.yml
  format: yaml
  label: Opkit Patients API
  slug: opkit-patients-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/opkit/refs/heads/main/openapi/opkit-patients-api-openapi.yml
- filename: opkit-payers-api-openapi.yml
  format: yaml
  label: Opkit Payers API
  slug: opkit-payers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/opkit/refs/heads/main/openapi/opkit-payers-api-openapi.yml
- filename: opkit-webhooks-api-openapi.yml
  format: yaml
  label: Opkit Webhooks API
  slug: opkit-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/opkit/refs/heads/main/openapi/opkit-webhooks-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Opkit Authentication
name_suffix: Authentication
oauth_flows: []
overview: Opkit secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Opkit
provider_slug: opkit
scheme_count: 1
schemes:
- description: 'Provide your Opkit API key as a Bearer token in the Authorization header: `Authorization: Bearer [example key]`.'
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/opkit-openapi.yml
  type: http
slug: opkit-authentication
source_filename: opkit-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/opkit-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  description: 'Provide your Opkit API key as a Bearer token in the Authorization header: `Authorization:\n    Bearer [example key]`.'\n  sources:\n  - openapi/opkit-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/opkit/refs/heads/main/authentication/opkit-authentication.yml
summary_line: http · 1 scheme
tags:
- Healthcare
- Insurance
- Eligibility
- Benefits
- Verification
- Telehealth
---
