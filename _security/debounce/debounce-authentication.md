---
api_key_in:
- query
api_specs:
- filename: debounce-email-validation-api-openapi.yml
  format: yaml
  label: DeBounce Email Validation API
  slug: email-validation-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/debounce/refs/heads/main/openapi/debounce-email-validation-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Debounce Authentication
name_suffix: Authentication
oauth_flows: []
overview: DeBounce secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: DeBounce
provider_slug: debounce
scheme_count: 1
schemes:
- description: DeBounce API key passed as the 'api' query parameter. Obtain your API key from the DeBounce account dashboard at https://app.debounce.io/.
  in: query
  name: ApiKeyQuery
  parameter: api
  sources:
  - openapi/debounce-email-validation-api-openapi.yml
  type: apiKey
slug: debounce-authentication
source_filename: debounce-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/debounce-email-validation-api-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - query\nschemes:\n- name: ApiKeyQuery\n  type: apiKey\n  in: query\n  parameter: api\n  description: DeBounce API key passed as the 'api' query parameter. Obtain your API key from\n    the DeBounce account dashboard at https://app.debounce.io/.\n  sources:\n  - openapi/debounce-email-validation-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/debounce/refs/heads/main/authentication/debounce-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Email Validation
- Email Verification
- Deliverability
- Disposable Email Detection
- MX Records
- Bulk Email Validation
- Data Enrichment
- Syntax Validation
---
