---
api_key_in: []
api_specs:
- filename: unitedhealthcare-claims-api-openapi.yml
  format: yaml
  label: UnitedHealthcare Claims API
  slug: unitedhealthcare-claims-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/unitedhealthcare/refs/heads/main/openapi/unitedhealthcare-claims-api-openapi.yml
- filename: unitedhealthcare-eligibility-api-openapi.yml
  format: yaml
  label: UnitedHealthcare Eligibility API
  slug: unitedhealthcare-eligibility-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/unitedhealthcare/refs/heads/main/openapi/unitedhealthcare-eligibility-api-openapi.yml
- filename: unitedhealthcare-formulary-api-openapi.yml
  format: yaml
  label: UnitedHealthcare Formulary API
  slug: unitedhealthcare-formulary-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/unitedhealthcare/refs/heads/main/openapi/unitedhealthcare-formulary-api-openapi.yml
- filename: unitedhealthcare-patient-access-api-openapi.yml
  format: yaml
  label: UnitedHealthcare Patient Access API
  slug: unitedhealthcare-patient-access-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/unitedhealthcare/refs/heads/main/openapi/unitedhealthcare-patient-access-api-openapi.yml
- filename: unitedhealthcare-prior-authorization-api-openapi.yml
  format: yaml
  label: UnitedHealthcare Prior Authorization API
  slug: unitedhealthcare-prior-authorization-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/unitedhealthcare/refs/heads/main/openapi/unitedhealthcare-prior-authorization-api-openapi.yml
- filename: unitedhealthcare-provider-directory-api-openapi.yml
  format: yaml
  label: UnitedHealthcare Provider Directory API
  slug: unitedhealthcare-provider-directory-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/unitedhealthcare/refs/heads/main/openapi/unitedhealthcare-provider-directory-api-openapi.yml
- filename: unitedhealthcare-providers-api-openapi.yml
  format: yaml
  label: UnitedHealthcare Providers API
  slug: unitedhealthcare-providers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/unitedhealthcare/refs/heads/main/openapi/unitedhealthcare-providers-api-openapi.yml
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
