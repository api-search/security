---
api_key_in: []
api_specs:
- filename: health-gorilla-openapi.yml
  format: yaml
  label: Patients (FHIR)
  slug: patients-fhir
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/health-gorilla/refs/heads/main/openapi/health-gorilla-openapi.yml
- filename: health-gorilla-openapi.yml
  format: yaml
  label: Record Query/Retrieval
  slug: record-query
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/health-gorilla/refs/heads/main/openapi/health-gorilla-openapi.yml
- filename: health-gorilla-openapi.yml
  format: yaml
  label: Lab Ordering
  slug: lab-ordering
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/health-gorilla/refs/heads/main/openapi/health-gorilla-openapi.yml
- filename: health-gorilla-openapi.yml
  format: yaml
  label: Diagnostic Reports
  slug: diagnostic-reports
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/health-gorilla/refs/heads/main/openapi/health-gorilla-openapi.yml
- filename: health-gorilla-openapi.yml
  format: yaml
  label: Documents
  slug: documents
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/health-gorilla/refs/heads/main/openapi/health-gorilla-openapi.yml
- filename: health-gorilla-openapi.yml
  format: yaml
  label: Eligibility
  slug: eligibility
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/health-gorilla/refs/heads/main/openapi/health-gorilla-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Health Gorilla Authentication
name_suffix: Authentication
oauth_flows: []
overview: Health Gorilla secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Health Gorilla
provider_slug: health-gorilla
scheme_count: 1
schemes:
- bearerFormat: JWT
  description: 'OAuth 2.0 bearer access token. Obtain a token using the client credentials issued during onboarding via the Health Gorilla OAuth 2.0 token endpoint, then pass it as `Authorization: Bearer {token}`.'
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/health-gorilla-openapi.yml
  type: http
slug: health-gorilla-authentication
source_filename: health-gorilla-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/health-gorilla-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  description: 'OAuth 2.0 bearer access token. Obtain a token using the client credentials issued\n    during onboarding via the Health Gorilla OAuth 2.0 token endpoint, then pass it as `Authorization:\n    Bearer {token}`.'\n  sources:\n  - openapi/health-gorilla-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/health-gorilla/refs/heads/main/authentication/health-gorilla-authentication.yml
summary_line: http · 1 scheme
tags:
- Health
- Interoperability
- FHIR
- Clinical Data
- Lab Ordering
---
