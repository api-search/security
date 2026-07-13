---
api_key_in: []
auth_types:
- oauth2
description: ''
kind: authentication
layout: security
method: derived
name: Google Cloud Healthcare Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
- implicit
overview: Google Cloud Healthcare secures its APIs with oauth2 across 2 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode and implicit flow(s).
provider_name: Google Cloud Healthcare
provider_slug: google-cloud-healthcare
scheme_count: 2
schemes:
- description: Oauth 2.0 implicit authentication
  flows:
  - authorizationUrl: https://accounts.google.com/o/oauth2/auth
    flow: implicit
    scopes: 2
  name: Oauth2
  sources:
  - openapi/openapi-v1.yaml
  - openapi/openapi-v1beta1.yaml
  type: oauth2
- description: Oauth 2.0 authorizationCode authentication
  flows:
  - authorizationUrl: https://accounts.google.com/o/oauth2/auth
    flow: authorizationCode
    scopes: 2
    tokenUrl: https://accounts.google.com/o/oauth2/token
  name: Oauth2c
  sources:
  - openapi/openapi-v1.yaml
  - openapi/openapi-v1beta1.yaml
  type: oauth2
slug: google-cloud-healthcare-authentication
source_filename: google-cloud-healthcare-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/openapi-v1.yaml, openapi/openapi-v1beta1.yaml\nsummary:\n  types:\n  - oauth2\n  oauth2_flows:\n  - authorizationCode\n  - implicit\nschemes:\n- name: Oauth2\n  type: oauth2\n  flows:\n  - flow: implicit\n    authorizationUrl: https://accounts.google.com/o/oauth2/auth\n    scopes: 2\n  description: Oauth 2.0 implicit authentication\n  sources:\n  - openapi/openapi-v1.yaml\n  - openapi/openapi-v1beta1.yaml\n- name: Oauth2c\n  type: oauth2\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://accounts.google.com/o/oauth2/auth\n    tokenUrl: https://accounts.google.com/o/oauth2/token\n    scopes: 2\n  description: Oauth 2.0 authorizationCode authentication\n  sources:\n  - openapi/openapi-v1.yaml\n  - openapi/openapi-v1beta1.yaml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/google-cloud-healthcare/refs/heads/main/authentication/google-cloud-healthcare-authentication.yml
summary_line: oauth2 · 2 schemes
tags:
- Healthcare
- FHIR
- HL7v2
- DICOM
- Medical Imaging
- De-identification
- Interoperability
- Cloud
---
