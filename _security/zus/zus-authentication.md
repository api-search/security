---
api_key_in: []
api_specs:
- filename: zus-auth-api-openapi.yml
  format: yaml
  label: Zus Health Auth API
  slug: zus-auth-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zus/refs/heads/main/openapi/zus-auth-api-openapi.yml
- filename: zus-documents-api-openapi.yml
  format: yaml
  label: Zus Health Documents API
  slug: zus-documents-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zus/refs/heads/main/openapi/zus-documents-api-openapi.yml
- filename: zus-fhir-api-openapi.yml
  format: yaml
  label: Zus Health FHIR API
  slug: zus-fhir-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zus/refs/heads/main/openapi/zus-fhir-api-openapi.yml
- filename: zus-patient-api-openapi.yml
  format: yaml
  label: Zus Health Patient API
  slug: zus-patient-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zus/refs/heads/main/openapi/zus-patient-api-openapi.yml
- filename: zus-patient-history-api-openapi.yml
  format: yaml
  label: Zus Health Patient History API
  slug: zus-patient-history-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zus/refs/heads/main/openapi/zus-patient-history-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Zus Authentication
name_suffix: Authentication
oauth_flows: []
overview: Zus Health secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Zus Health
provider_slug: zus
scheme_count: 1
schemes:
- bearerFormat: JWT
  description: 'OAuth2 Bearer access token obtained from the Zus token endpoint (auth.zusapi.com/oauth/token). Sent as Authorization: Bearer <ACCESS_TOKEN>.'
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/zus-openapi.yml
  type: http
slug: zus-authentication
source_filename: zus-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/zus-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  description: 'OAuth2 Bearer access token obtained from the Zus token endpoint (auth.zusapi.com/oauth/token).\n    Sent as Authorization: Bearer <ACCESS_TOKEN>.'\n  sources:\n  - openapi/zus-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/zus/refs/heads/main/authentication/zus-authentication.yml
summary_line: http · 1 scheme
tags:
- Health
- FHIR
- Interoperability
- Patient Data
- Healthcare
---
