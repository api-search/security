---
api_key_in: []
api_specs:
- filename: penn-medicine-fhir-r4-openapi.yml
  format: yaml
  label: Penn Medicine FHIR R4 API
  slug: penn-medicine-fhir-r4-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/penn-medicine/refs/heads/main/openapi/penn-medicine-fhir-r4-openapi.yml
auth_types:
- oauth2
description: ''
kind: authentication
layout: security
method: derived
name: Penn Medicine Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
- clientCredentials
overview: Penn Medicine secures its APIs with oauth2 across 1 declared security scheme, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode and clientCredentials flow(s).
provider_name: Penn Medicine
provider_slug: penn-medicine
scheme_count: 1
schemes:
- flows:
  - authorizationUrl: https://ssproxy.pennhealth.com/PRD-FHIR/oauth2/authorize
    flow: authorizationCode
    scopes: 5
    tokenUrl: https://ssproxy.pennhealth.com/PRD-FHIR/oauth2/token
  - flow: clientCredentials
    scopes: 1
    tokenUrl: https://ssproxy.pennhealth.com/PRD-FHIR/oauth2/token
  name: smartOnFhir
  sources:
  - openapi/penn-medicine-fhir-r4-openapi.yml
  type: oauth2
slug: penn-medicine-authentication
source_filename: penn-medicine-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/penn-medicine-fhir-r4-openapi.yml\nsummary:\n  types:\n  - oauth2\n  oauth2_flows:\n  - authorizationCode\n  - clientCredentials\nschemes:\n- name: smartOnFhir\n  type: oauth2\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://ssproxy.pennhealth.com/PRD-FHIR/oauth2/authorize\n    tokenUrl: https://ssproxy.pennhealth.com/PRD-FHIR/oauth2/token\n    scopes: 5\n  - flow: clientCredentials\n    tokenUrl: https://ssproxy.pennhealth.com/PRD-FHIR/oauth2/token\n    scopes: 1\n  sources:\n  - openapi/penn-medicine-fhir-r4-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/penn-medicine/refs/heads/main/authentication/penn-medicine-authentication.yml
summary_line: oauth2 · 1 scheme
tags:
- Healthcare
- Hospital
- Academic Medical Center
- FHIR
- SMART On FHIR
- Patient Access
- Provider Directory
- CMS Interoperability
- US Core
- Bulk Data
- Epic
---
