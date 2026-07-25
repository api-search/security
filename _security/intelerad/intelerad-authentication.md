---
api_key_in:
- query
api_specs:
- filename: intelerad-hl7-api-openapi.yml
  format: yaml
  label: Intelerad HL7 API
  slug: intelerad-hl7-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/intelerad/refs/heads/main/openapi/intelerad-hl7-api-openapi.yml
- filename: intelerad-namespace-api-openapi.yml
  format: yaml
  label: Intelerad Namespace API
  slug: intelerad-namespace-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/intelerad/refs/heads/main/openapi/intelerad-namespace-api-openapi.yml
- filename: intelerad-order-api-openapi.yml
  format: yaml
  label: Intelerad Order API
  slug: intelerad-order-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/intelerad/refs/heads/main/openapi/intelerad-order-api-openapi.yml
- filename: intelerad-patient-api-openapi.yml
  format: yaml
  label: Intelerad Patient API
  slug: intelerad-patient-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/intelerad/refs/heads/main/openapi/intelerad-patient-api-openapi.yml
- filename: intelerad-report-api-openapi.yml
  format: yaml
  label: Intelerad Report API
  slug: intelerad-report-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/intelerad/refs/heads/main/openapi/intelerad-report-api-openapi.yml
- filename: intelerad-session-api-openapi.yml
  format: yaml
  label: Intelerad Session API
  slug: intelerad-session-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/intelerad/refs/heads/main/openapi/intelerad-session-api-openapi.yml
- filename: intelerad-storage-api-openapi.yml
  format: yaml
  label: Intelerad Storage API
  slug: intelerad-storage-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/intelerad/refs/heads/main/openapi/intelerad-storage-api-openapi.yml
- filename: intelerad-study-api-openapi.yml
  format: yaml
  label: Intelerad Study API
  slug: intelerad-study-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/intelerad/refs/heads/main/openapi/intelerad-study-api-openapi.yml
- filename: intelerad-webhook-api-openapi.yml
  format: yaml
  label: Intelerad Webhook API
  slug: intelerad-webhook-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/intelerad/refs/heads/main/openapi/intelerad-webhook-api-openapi.yml
auth_types:
- apiKey
- http
description: ''
kind: authentication
layout: security
method: derived
name: Intelerad Authentication
name_suffix: Authentication
oauth_flows: []
overview: Intelerad secures its APIs with apiKey and http across 3 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Intelerad
provider_slug: intelerad
scheme_count: 3
schemes:
- description: Session id obtained from /session/login. May also be supplied as a request field depending on the endpoint.
  in: query
  name: sid
  parameter: sid
  sources:
  - openapi/intelerad-openapi.yml
  type: apiKey
- name: basicAuth
  scheme: basic
  sources:
  - openapi/intelerad-openapi.yml
  type: http
- description: OAuth bearer token for third-party integrations.
  name: oauth
  scheme: bearer
  sources:
  - openapi/intelerad-openapi.yml
  type: http
slug: intelerad-authentication
source_filename: intelerad-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/intelerad-openapi.yml\nsummary:\n  types:\n  - apiKey\n  - http\n  api_key_in:\n  - query\nschemes:\n- name: sid\n  type: apiKey\n  in: query\n  parameter: sid\n  description: Session id obtained from /session/login. May also be supplied as a request field\n    depending on the endpoint.\n  sources:\n  - openapi/intelerad-openapi.yml\n- name: basicAuth\n  type: http\n  scheme: basic\n  sources:\n  - openapi/intelerad-openapi.yml\n- name: oauth\n  type: http\n  scheme: bearer\n  description: OAuth bearer token for third-party integrations.\n  sources:\n  - openapi/intelerad-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/intelerad/refs/heads/main/authentication/intelerad-authentication.yml
summary_line: apiKey/http · 3 schemes
tags:
- Medical Imaging
- PACS
- Enterprise Imaging
- Radiology
- DICOM
- DICOMweb
- HL7
- FHIR
- Healthcare
- Interoperability
- Image Exchange
---
