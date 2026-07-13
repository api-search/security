---
api_key_in: []
api_specs:
- filename: zus-openapi.yml
  format: yaml
  label: Zus Patients (FHIR)
  slug: patients-fhir
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zus/refs/heads/main/openapi/zus-openapi.yml
- filename: zus-openapi.yml
  format: yaml
  label: Zus Aggregated Profile
  slug: aggregated-profile
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zus/refs/heads/main/openapi/zus-openapi.yml
- filename: zus-openapi.yml
  format: yaml
  label: Zus FHIR Resources
  slug: fhir-resources
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zus/refs/heads/main/openapi/zus-openapi.yml
- filename: zus-openapi.yml
  format: yaml
  label: Zus Document Retrieval
  slug: document-retrieval
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zus/refs/heads/main/openapi/zus-openapi.yml
- filename: zus-openapi.yml
  format: yaml
  label: Zus Subscriptions and Webhooks
  slug: subscriptions-webhooks
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zus/refs/heads/main/openapi/zus-openapi.yml
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
