---
api_key_in: []
api_specs:
- filename: medplum-openapi-original.yml
  format: yaml
  label: Medplum FHIR REST API
  slug: medplum-fhir-rest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/medplum/refs/heads/main/openapi/medplum-openapi-original.yml
auth_types:
- http
- openIdConnect
description: ''
kind: authentication
layout: security
method: derived
name: Medplum Authentication
name_suffix: Authentication
oauth_flows: []
overview: Medplum secures its APIs with http and openIdConnect across 3 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Medplum
provider_slug: medplum
scheme_count: 3
schemes:
- name: BasicAuth
  scheme: basic
  sources:
  - openapi/medplum-openapi-original.yml
  type: http
- bearerFormat: JWT
  name: BearerAuth
  scheme: bearer
  sources:
  - openapi/medplum-openapi-original.yml
  type: http
- name: OpenID
  openIdConnectUrl: https://api.medplum.com/.well-known/openid-configuration
  sources:
  - openapi/medplum-openapi-original.yml
  type: openIdConnect
slug: medplum-authentication
source_filename: medplum-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/medplum-openapi-original.yml\nsummary:\n  types:\n  - http\n  - openIdConnect\nschemes:\n- name: BasicAuth\n  type: http\n  scheme: basic\n  sources:\n  - openapi/medplum-openapi-original.yml\n- name: BearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  sources:\n  - openapi/medplum-openapi-original.yml\n- name: OpenID\n  type: openIdConnect\n  openIdConnectUrl: https://api.medplum.com/.well-known/openid-configuration\n  sources:\n  - openapi/medplum-openapi-original.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/medplum/refs/heads/main/authentication/medplum-authentication.yml
summary_line: http/openIdConnect · 3 schemes
tags:
- Healthcare
- FHIR
- Open Source
- Developer Platform
- HIPAA
- SMART on FHIR
- Clinical
- Interoperability
---
