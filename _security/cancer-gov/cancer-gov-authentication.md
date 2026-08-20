---
api_key_in:
- header
api_specs:
- filename: cancer-gov-diseases-api-openapi.yml
  format: yaml
  label: Cancer.gov Diseases API
  slug: cancer-gov-diseases-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cancer-gov/refs/heads/main/openapi/cancer-gov-diseases-api-openapi.yml
- filename: cancer-gov-interventions-api-openapi.yml
  format: yaml
  label: Cancer.gov Interventions API
  slug: cancer-gov-interventions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cancer-gov/refs/heads/main/openapi/cancer-gov-interventions-api-openapi.yml
- filename: cancer-gov-terms-api-openapi.yml
  format: yaml
  label: Cancer.gov Terms API
  slug: cancer-gov-terms-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cancer-gov/refs/heads/main/openapi/cancer-gov-terms-api-openapi.yml
- filename: cancer-gov-trials-api-openapi.yml
  format: yaml
  label: Cancer.gov Trials API
  slug: cancer-gov-trials-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cancer-gov/refs/heads/main/openapi/cancer-gov-trials-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Cancer Gov Authentication
name_suffix: Authentication
oauth_flows: []
overview: Cancer.gov secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Cancer.gov
provider_slug: cancer-gov
scheme_count: 1
schemes:
- description: Free API key issued by the CTS Developer Accounts portal.
  in: header
  name: apiKey
  parameter: X-API-KEY
  sources:
  - openapi/cancer-gov-openapi.yml
  type: apiKey
slug: cancer-gov-authentication
source_filename: cancer-gov-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/cancer-gov-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: apiKey\n  type: apiKey\n  in: header\n  parameter: X-API-KEY\n  description: Free API key issued by the CTS Developer Accounts portal.\n  sources:\n  - openapi/cancer-gov-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/cancer-gov/refs/heads/main/authentication/cancer-gov-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Cancer
- Federal-Government
- Healthcare
- Research
- Clinical Trials
- Genomics
- Surveillance
- Open Data
---
