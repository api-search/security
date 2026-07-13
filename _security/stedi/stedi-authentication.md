---
api_key_in:
- header
api_specs:
- filename: core.json
  format: json
  label: Stedi Core API
  slug: stedi-core-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/Stedi/openApi/main/core.json
- filename: healthcare.json
  format: json
  label: Stedi Healthcare Eligibility API
  slug: stedi-healthcare-eligibility-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/Stedi/openApi/main/healthcare.json
- filename: claims.json
  format: json
  label: Stedi Claims API
  slug: stedi-claims-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/Stedi/openApi/main/claims.json
- filename: payers.json
  format: json
  label: Stedi Payers API
  slug: stedi-payers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/Stedi/openApi/main/payers.json
- filename: enrollment.json
  format: json
  label: Stedi Enrollment API
  slug: stedi-enrollment-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/Stedi/openApi/main/enrollment.json
- filename: event-destinations.json
  format: json
  label: Stedi Event Destinations API
  slug: stedi-event-destinations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/Stedi/openApi/main/event-destinations.json
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Stedi Authentication
name_suffix: Authentication
oauth_flows: []
overview: Stedi secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Stedi
provider_slug: stedi
scheme_count: 1
schemes:
- description: A [Stedi API Key](https://www.stedi.com/app/settings/api-keys) for authentication.
  in: header
  name: httpApiKeyAuth
  parameter: Authorization
  sources:
  - openapi/stedi-claims-openapi.yml
  - openapi/stedi-core-openapi.yml
  - openapi/stedi-enrollment-openapi.yml
  - openapi/stedi-event-destinations-openapi.yml
  - openapi/stedi-healthcare-openapi.yml
  - openapi/stedi-payers-openapi.yml
  type: apiKey
slug: stedi-authentication
source_filename: stedi-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/stedi-claims-openapi.yml, openapi/stedi-core-openapi.yml, openapi/stedi-enrollment-openapi.yml,\n  openapi/stedi-event-destinations-openapi.yml, openapi/stedi-healthcare-openapi.yml, openapi/stedi-payers-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: httpApiKeyAuth\n  type: apiKey\n  in: header\n  parameter: Authorization\n  description: A [Stedi API Key](https://www.stedi.com/app/settings/api-keys) for authentication.\n  sources:\n  - openapi/stedi-claims-openapi.yml\n  - openapi/stedi-core-openapi.yml\n  - openapi/stedi-enrollment-openapi.yml\n  - openapi/stedi-event-destinations-openapi.yml\n  - openapi/stedi-healthcare-openapi.yml\n  - openapi/stedi-payers-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/stedi/refs/heads/main/authentication/stedi-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- EDI
- Electronic Data Interchange
- Healthcare
- Clearinghouse
- X12
- Claims
- Eligibility
- HIPAA
- Revenue Cycle Management
- B2B Integration
---
