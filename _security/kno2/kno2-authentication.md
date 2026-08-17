---
api_key_in: []
api_specs:
- filename: kno2-attachments-api-openapi.yml
  format: yaml
  label: Kno2 Attachments API
  slug: kno2-attachments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kno2/refs/heads/main/openapi/kno2-attachments-api-openapi.yml
- filename: kno2-authentication-api-openapi.yml
  format: yaml
  label: Kno2 Authentication API
  slug: kno2-authentication-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kno2/refs/heads/main/openapi/kno2-authentication-api-openapi.yml
- filename: kno2-directory-api-openapi.yml
  format: yaml
  label: Kno2 Directory API
  slug: kno2-directory-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kno2/refs/heads/main/openapi/kno2-directory-api-openapi.yml
- filename: kno2-intake-api-openapi.yml
  format: yaml
  label: Kno2 Intake API
  slug: kno2-intake-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kno2/refs/heads/main/openapi/kno2-intake-api-openapi.yml
- filename: kno2-messaging-api-openapi.yml
  format: yaml
  label: Kno2 Messaging API
  slug: kno2-messaging-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kno2/refs/heads/main/openapi/kno2-messaging-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Kno2 Authentication
name_suffix: Authentication
oauth_flows: []
overview: Kno2 secures its APIs with http across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Kno2
provider_slug: kno2
scheme_count: 2
schemes:
- description: Bearer access token obtained from POST /api/token.
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/kno2-attachments-api-openapi.yml
  - openapi/kno2-authentication-api-openapi.yml
  - openapi/kno2-directory-api-openapi.yml
  - openapi/kno2-intake-api-openapi.yml
  - openapi/kno2-messaging-api-openapi.yml
  type: http
- description: HTTP Basic with base64(client_id:client_secret), used only against /api/token to obtain a Bearer token.
  name: basicAuth
  scheme: basic
  sources:
  - openapi/kno2-attachments-api-openapi.yml
  - openapi/kno2-authentication-api-openapi.yml
  - openapi/kno2-directory-api-openapi.yml
  - openapi/kno2-intake-api-openapi.yml
  - openapi/kno2-messaging-api-openapi.yml
  type: http
slug: kno2-authentication
source_filename: kno2-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-14'\nmethod: derived\nsource: openapi/kno2-attachments-api-openapi.yml, openapi/kno2-authentication-api-openapi.yml,\n  openapi/kno2-directory-api-openapi.yml, openapi/kno2-intake-api-openapi.yml, openapi/kno2-messaging-api-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  description: Bearer access token obtained from POST /api/token.\n  sources:\n  - openapi/kno2-attachments-api-openapi.yml\n  - openapi/kno2-authentication-api-openapi.yml\n  - openapi/kno2-directory-api-openapi.yml\n  - openapi/kno2-intake-api-openapi.yml\n  - openapi/kno2-messaging-api-openapi.yml\n- name: basicAuth\n  type: http\n  scheme: basic\n  description: HTTP Basic with base64(client_id:client_secret), used only against /api/token\n    to obtain a Bearer token.\n  sources:\n  - openapi/kno2-attachments-api-openapi.yml\n  - openapi/kno2-authentication-api-openapi.yml\n  - openapi/kno2-directory-api-openapi.yml\n  - openapi/kno2-intake-api-openapi.yml\n\
  \  - openapi/kno2-messaging-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/kno2/refs/heads/main/authentication/kno2-authentication.yml
summary_line: http · 2 schemes
tags:
- Healthcare Interoperability
- Clinical Records
- Health Information Exchange
- Direct Secure Messaging
- FHIR
- Clinical Documents
- Patient Records
- Healthcare
- HIE
- Care Coordination
- QHIN
- TEFCA
- Carequality
---
