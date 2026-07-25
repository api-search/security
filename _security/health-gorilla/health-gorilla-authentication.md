---
api_key_in: []
api_specs:
- filename: health-gorilla-binary-api-openapi.yml
  format: yaml
  label: Health Gorilla Binary API
  slug: health-gorilla-binary-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/health-gorilla/refs/heads/main/openapi/health-gorilla-binary-api-openapi.yml
- filename: health-gorilla-capabilitystatement-api-openapi.yml
  format: yaml
  label: Health Gorilla CapabilityStatement API
  slug: health-gorilla-capabilitystatement-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/health-gorilla/refs/heads/main/openapi/health-gorilla-capabilitystatement-api-openapi.yml
- filename: health-gorilla-coverage-api-openapi.yml
  format: yaml
  label: Health Gorilla Coverage API
  slug: health-gorilla-coverage-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/health-gorilla/refs/heads/main/openapi/health-gorilla-coverage-api-openapi.yml
- filename: health-gorilla-diagnosticreport-api-openapi.yml
  format: yaml
  label: Health Gorilla DiagnosticReport API
  slug: health-gorilla-diagnosticreport-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/health-gorilla/refs/heads/main/openapi/health-gorilla-diagnosticreport-api-openapi.yml
- filename: health-gorilla-documentreference-api-openapi.yml
  format: yaml
  label: Health Gorilla DocumentReference API
  slug: health-gorilla-documentreference-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/health-gorilla/refs/heads/main/openapi/health-gorilla-documentreference-api-openapi.yml
- filename: health-gorilla-observation-api-openapi.yml
  format: yaml
  label: Health Gorilla Observation API
  slug: health-gorilla-observation-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/health-gorilla/refs/heads/main/openapi/health-gorilla-observation-api-openapi.yml
- filename: health-gorilla-patient-api-openapi.yml
  format: yaml
  label: Health Gorilla Patient API
  slug: health-gorilla-patient-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/health-gorilla/refs/heads/main/openapi/health-gorilla-patient-api-openapi.yml
- filename: health-gorilla-practitioner-api-openapi.yml
  format: yaml
  label: Health Gorilla Practitioner API
  slug: health-gorilla-practitioner-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/health-gorilla/refs/heads/main/openapi/health-gorilla-practitioner-api-openapi.yml
- filename: health-gorilla-requestgroup-api-openapi.yml
  format: yaml
  label: Health Gorilla RequestGroup API
  slug: health-gorilla-requestgroup-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/health-gorilla/refs/heads/main/openapi/health-gorilla-requestgroup-api-openapi.yml
- filename: health-gorilla-servicerequest-api-openapi.yml
  format: yaml
  label: Health Gorilla ServiceRequest API
  slug: health-gorilla-servicerequest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/health-gorilla/refs/heads/main/openapi/health-gorilla-servicerequest-api-openapi.yml
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
