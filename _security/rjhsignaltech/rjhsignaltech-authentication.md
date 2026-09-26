---
anonymous_access: false
api_key_in:
- header
api_specs:
- filename: rjhsignaltech-batch-api-openapi.yml
  format: yaml
  label: Who Represents This Address (RJH Signal Technologies) Batch API
  slug: rjhsignaltech-batch-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/rjhsignaltech/refs/heads/main/openapi/rjhsignaltech-batch-api-openapi.yml
- filename: rjhsignaltech-civicinfo-api-openapi.yml
  format: yaml
  label: Who Represents This Address (RJH Signal Technologies) Civicinfo API
  slug: rjhsignaltech-civicinfo-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/rjhsignaltech/refs/heads/main/openapi/rjhsignaltech-civicinfo-api-openapi.yml
- filename: rjhsignaltech-divisions-api-openapi.yml
  format: yaml
  label: Who Represents This Address (RJH Signal Technologies) Divisions API
  slug: rjhsignaltech-divisions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/rjhsignaltech/refs/heads/main/openapi/rjhsignaltech-divisions-api-openapi.yml
- filename: rjhsignaltech-lookup-api-openapi.yml
  format: yaml
  label: Who Represents This Address (RJH Signal Technologies) Lookup API
  slug: rjhsignaltech-lookup-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/rjhsignaltech/refs/heads/main/openapi/rjhsignaltech-lookup-api-openapi.yml
- filename: rjhsignaltech-x402-api-openapi.yml
  format: yaml
  label: Who Represents This Address (RJH Signal Technologies) X402 API
  slug: rjhsignaltech-x402-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/rjhsignaltech/refs/heads/main/openapi/rjhsignaltech-x402-api-openapi.yml
- filename: rjhsignaltech-zip-api-openapi.yml
  format: yaml
  label: Who Represents This Address (RJH Signal Technologies) Zip API
  slug: rjhsignaltech-zip-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/rjhsignaltech/refs/heads/main/openapi/rjhsignaltech-zip-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: derived
name: Rjhsignaltech Authentication
name_suffix: Authentication
oauth_flows: []
overview: Who Represents This Address (RJH Signal Technologies) secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Who Represents This Address (RJH Signal Technologies)
provider_slug: rjhsignaltech
scheme_count: 1
schemes:
- in: header
  name: apiKey
  parameter: X-API-Key
  sources:
  - openapi/whorepresents.openapi.json
  type: apiKey
slug: rjhsignaltech-authentication
source_filename: rjhsignaltech-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-09-25'\nmethod: derived\nsource: openapi/whorepresents.openapi.json\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: apiKey\n  type: apiKey\n  in: header\n  parameter: X-API-Key\n  sources:\n  - openapi/whorepresents.openapi.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/rjhsignaltech/refs/heads/main/authentication/rjhsignaltech-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Company
- API
- Civic
- Government
- Address
---
