---
api_key_in: []
api_specs:
- filename: canvas-medical-fhir-api-openapi.yml
  format: yaml
  label: Canvas Medical FHIR API
  slug: canvas-medical-fhir-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/canvas-medical/refs/heads/main/openapi/canvas-medical-fhir-api-openapi.yml
auth_types:
- http
- oauth2
description: ''
kind: authentication
layout: security
method: derived
name: Canvas Medical Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
- clientCredentials
overview: Canvas Medical secures its APIs with http and oauth2 across 3 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode and clientCredentials flow(s).
provider_name: Canvas Medical
provider_slug: canvas-medical
scheme_count: 3
schemes:
- description: Machine-to-machine authentication using client credentials grant. Obtain client_id and client_secret from Canvas admin panel.
  flows:
  - flow: clientCredentials
    scopes: 8
    tokenUrl: https://{canvas-instance}.canvasmedical.com/auth/token/
  name: OAuth2ClientCredentials
  sources:
  - openapi/canvas-medical-fhir-api-openapi.yml
  type: oauth2
- description: User-delegated access using Authorization Code flow with SMART on FHIR scopes.
  flows:
  - authorizationUrl: https://{canvas-instance}.canvasmedical.com/auth/authorize/
    flow: authorizationCode
    scopes: 3
    tokenUrl: https://{canvas-instance}.canvasmedical.com/auth/token/
  name: OAuth2AuthCode
  sources:
  - openapi/canvas-medical-fhir-api-openapi.yml
  type: oauth2
- bearerFormat: JWT
  name: BearerAuth
  scheme: bearer
  sources:
  - openapi/canvas-medical-fhir-api-openapi.yml
  type: http
slug: canvas-medical-authentication
source_filename: canvas-medical-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/canvas-medical-fhir-api-openapi.yml\nsummary:\n  types:\n  - http\n  - oauth2\n  oauth2_flows:\n  - authorizationCode\n  - clientCredentials\nschemes:\n- name: OAuth2ClientCredentials\n  type: oauth2\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://{canvas-instance}.canvasmedical.com/auth/token/\n    scopes: 8\n  description: Machine-to-machine authentication using client credentials grant. Obtain client_id\n    and client_secret from Canvas admin panel.\n  sources:\n  - openapi/canvas-medical-fhir-api-openapi.yml\n- name: OAuth2AuthCode\n  type: oauth2\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://{canvas-instance}.canvasmedical.com/auth/authorize/\n    tokenUrl: https://{canvas-instance}.canvasmedical.com/auth/token/\n    scopes: 3\n  description: User-delegated access using Authorization Code flow with SMART on FHIR scopes.\n  sources:\n  - openapi/canvas-medical-fhir-api-openapi.yml\n\
  - name: BearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  sources:\n  - openapi/canvas-medical-fhir-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/canvas-medical/refs/heads/main/authentication/canvas-medical-authentication.yml
summary_line: http/oauth2 · 3 schemes
tags:
- EHR
- FHIR
- Healthcare
- Electronic Health Records
- Virtual Care
- Clinical Workflows
- Patient Management
- Care Coordination
---
