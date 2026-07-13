---
api_key_in: []
api_specs:
- filename: hhaexchange-fhir-openapi.yml
  format: yaml
  label: HHAeXchange EVV API
  slug: hhaexchange-evv-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hhaexchange/refs/heads/main/openapi/hhaexchange-fhir-openapi.yml
auth_types:
- oauth2
description: ''
kind: authentication
layout: security
method: derived
name: Hhaexchange Authentication
name_suffix: Authentication
oauth_flows:
- clientCredentials
overview: HHAeXchange secures its APIs with oauth2 across 1 declared security scheme, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the clientCredentials flow(s).
provider_name: HHAeXchange
provider_slug: hhaexchange
scheme_count: 1
schemes:
- flows:
  - flow: clientCredentials
    scopes: 1
    tokenUrl: https://api.hhaexchange.com/v1/fhir/auth/token
  name: bearerAuth
  sources:
  - openapi/hhaexchange-fhir-openapi.yml
  type: oauth2
slug: hhaexchange-authentication
source_filename: hhaexchange-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/hhaexchange-fhir-openapi.yml\nsummary:\n  types:\n  - oauth2\n  oauth2_flows:\n  - clientCredentials\nschemes:\n- name: bearerAuth\n  type: oauth2\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://api.hhaexchange.com/v1/fhir/auth/token\n    scopes: 1\n  sources:\n  - openapi/hhaexchange-fhir-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/hhaexchange/refs/heads/main/authentication/hhaexchange-authentication.yml
summary_line: oauth2 · 1 scheme
tags:
- Homecare
- EVV
- Electronic Visit Verification
- Medicaid
- Scheduling
- Caregiver
- Healthcare
---
