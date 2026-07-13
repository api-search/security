---
api_key_in: []
api_specs:
- filename: unitedhealthcare-provider-api-openapi.yml
  format: yaml
  label: UnitedHealthcare Provider API
  slug: provider-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/unitedhealthcare/refs/heads/main/openapi/unitedhealthcare-provider-api-openapi.yml
- filename: unitedhealthcare-interoperability-api-openapi.yml
  format: yaml
  label: UnitedHealthcare Interoperability API
  slug: interoperability-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/unitedhealthcare/refs/heads/main/openapi/unitedhealthcare-interoperability-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Unitedhealthcare Authentication
name_suffix: Authentication
oauth_flows: []
overview: UnitedHealthcare secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: UnitedHealthcare
provider_slug: unitedhealthcare
scheme_count: 1
schemes:
- description: OAuth 2.0 Bearer token for FHIR API access
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/unitedhealthcare-interoperability-api-openapi.yml
  - openapi/unitedhealthcare-provider-api-openapi.yml
  type: http
slug: unitedhealthcare-authentication
source_filename: unitedhealthcare-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/unitedhealthcare-interoperability-api-openapi.yml, openapi/unitedhealthcare-provider-api-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  description: OAuth 2.0 Bearer token for FHIR API access\n  sources:\n  - openapi/unitedhealthcare-interoperability-api-openapi.yml\n  - openapi/unitedhealthcare-provider-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/unitedhealthcare/refs/heads/main/authentication/unitedhealthcare-authentication.yml
summary_line: http · 1 scheme
tags:
- Health Insurance
- Healthcare
- FHIR
- Claims
- Eligibility
---
