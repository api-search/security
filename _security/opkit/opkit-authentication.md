---
api_key_in: []
api_specs:
- filename: opkit-openapi.yml
  format: yaml
  label: Opkit Eligibility Inquiries API
  slug: eligibility-inquiries
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/opkit/refs/heads/main/openapi/opkit-openapi.yml
- filename: opkit-openapi.yml
  format: yaml
  label: Opkit Benefits API
  slug: benefits
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/opkit/refs/heads/main/openapi/opkit-openapi.yml
- filename: opkit-openapi.yml
  format: yaml
  label: Opkit Payers API
  slug: payers
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/opkit/refs/heads/main/openapi/opkit-openapi.yml
- filename: opkit-openapi.yml
  format: yaml
  label: Opkit Patients API
  slug: patients
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/opkit/refs/heads/main/openapi/opkit-openapi.yml
- filename: opkit-openapi.yml
  format: yaml
  label: Opkit Webhooks API
  slug: webhooks
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/opkit/refs/heads/main/openapi/opkit-openapi.yml
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
- description: 'Provide your Opkit API key as a Bearer token in the Authorization header: `Authorization: Bearer YOUR_API_KEY`.'
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/opkit-openapi.yml
  type: http
slug: opkit-authentication
source_filename: opkit-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/opkit-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  description: 'Provide your Opkit API key as a Bearer token in the Authorization header: `Authorization:\n    Bearer YOUR_API_KEY`.'\n  sources:\n  - openapi/opkit-openapi.yml\n"
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
