---
api_key_in: []
api_specs:
- filename: varian-aria-fhir-openapi.yml
  format: yaml
  label: ARIA FHIR API
  slug: aria-fhir-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/varian-medical-systems/refs/heads/main/openapi/varian-aria-fhir-openapi.yml
auth_types:
- oauth2
description: ''
kind: authentication
layout: security
method: derived
name: Varian Medical Systems Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: Varian Medical Systems secures its APIs with oauth2 across 1 declared security scheme, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: Varian Medical Systems
provider_slug: varian-medical-systems
scheme_count: 1
schemes:
- description: SMART on FHIR OAuth 2.0 authorization
  flows:
  - authorizationUrl: https://varian-smart.dynamicfhir.com/core/connect/authorize
    flow: authorizationCode
    scopes: 11
    tokenUrl: https://varian-smart.dynamicfhir.com/core/connect/token
  name: OAuthSMARTonFHIR
  sources:
  - openapi/varian-aria-fhir-openapi.yml
  type: oauth2
slug: varian-medical-systems-authentication
source_filename: varian-medical-systems-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/varian-aria-fhir-openapi.yml\nsummary:\n  types:\n  - oauth2\n  oauth2_flows:\n  - authorizationCode\nschemes:\n- name: OAuthSMARTonFHIR\n  type: oauth2\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://varian-smart.dynamicfhir.com/core/connect/authorize\n    tokenUrl: https://varian-smart.dynamicfhir.com/core/connect/token\n    scopes: 11\n  description: SMART on FHIR OAuth 2.0 authorization\n  sources:\n  - openapi/varian-aria-fhir-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/varian-medical-systems/refs/heads/main/authentication/varian-medical-systems-authentication.yml
summary_line: oauth2 · 1 scheme
tags:
- Healthcare
- Oncology
- Medical Devices
- FHIR
- Radiation Therapy
- Health IT
- Fortune 1000
---
