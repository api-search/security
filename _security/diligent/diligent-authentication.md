---
api_key_in:
- header
api_specs:
- filename: diligent-cdd-api-openapi.yml
  format: yaml
  label: Diligent CDD API
  slug: diligent-cdd-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/diligent/refs/heads/main/openapi/diligent-cdd-api-openapi.yml
- filename: diligent-company-api-openapi.yml
  format: yaml
  label: Diligent Company API
  slug: diligent-company-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/diligent/refs/heads/main/openapi/diligent-company-api-openapi.yml
- filename: diligent-instant-screening-experimental-api-openapi.yml
  format: yaml
  label: Diligent Instant Screening (experimental) API
  slug: diligent-instant-screening-experimental-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/diligent/refs/heads/main/openapi/diligent-instant-screening-experimental-api-openapi.yml
- filename: diligent-monitorings-api-openapi.yml
  format: yaml
  label: Diligent Monitorings API
  slug: diligent-monitorings-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/diligent/refs/heads/main/openapi/diligent-monitorings-api-openapi.yml
- filename: diligent-name-screening-api-openapi.yml
  format: yaml
  label: Diligent Name Screening API
  slug: diligent-name-screening-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/diligent/refs/heads/main/openapi/diligent-name-screening-api-openapi.yml
- filename: diligent-webhooks-api-openapi.yml
  format: yaml
  label: Diligent Webhooks API
  slug: diligent-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/diligent/refs/heads/main/openapi/diligent-webhooks-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Diligent Authentication
name_suffix: Authentication
oauth_flows: []
overview: Diligent secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Diligent
provider_slug: diligent
scheme_count: 1
schemes:
- in: header
  name: xApiKey
  parameter: X-API-KEY
  sources:
  - openapi/diligent-openapi-original.json
  - openapi/diligent-remediation-openapi.json
  type: apiKey
slug: diligent-authentication
source_filename: diligent-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: derived\nsource: openapi/diligent-openapi-original.json, openapi/diligent-remediation-openapi.json\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: xApiKey\n  type: apiKey\n  in: header\n  parameter: X-API-KEY\n  sources:\n  - openapi/diligent-openapi-original.json\n  - openapi/diligent-remediation-openapi.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/diligent/refs/heads/main/authentication/diligent-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Company
- Compliance
- RegTech
- KYC
- AML
- Financial Crime
- Due Diligence
- Screening
- Sanctions
- Monitoring
- Artificial Intelligence
- Fintech
- Webhook
---
