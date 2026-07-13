---
api_key_in:
- query
api_specs:
- filename: intelerad-openapi.yml
  format: yaml
  label: InteleShare Studies API
  slug: intelerad-studies-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/intelerad/refs/heads/main/openapi/intelerad-openapi.yml
- filename: intelerad-openapi.yml
  format: yaml
  label: InteleShare Storage API
  slug: intelerad-storage-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/intelerad/refs/heads/main/openapi/intelerad-openapi.yml
- filename: intelerad-openapi.yml
  format: yaml
  label: InteleShare Patients API
  slug: intelerad-patients-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/intelerad/refs/heads/main/openapi/intelerad-openapi.yml
- filename: intelerad-openapi.yml
  format: yaml
  label: InteleShare Orders and Worklist API
  slug: intelerad-worklist-orders-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/intelerad/refs/heads/main/openapi/intelerad-openapi.yml
- filename: intelerad-openapi.yml
  format: yaml
  label: InteleShare Reports API
  slug: intelerad-reports-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/intelerad/refs/heads/main/openapi/intelerad-openapi.yml
- filename: intelerad-openapi.yml
  format: yaml
  label: InteleShare HL7 Integration API
  slug: intelerad-hl7-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/intelerad/refs/heads/main/openapi/intelerad-openapi.yml
- filename: intelerad-openapi.yml
  format: yaml
  label: InteleShare Webhooks and Routing API
  slug: intelerad-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/intelerad/refs/heads/main/openapi/intelerad-openapi.yml
- filename: intelerad-openapi.yml
  format: yaml
  label: InteleShare Namespaces and Accounts API
  slug: intelerad-namespaces-accounts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/intelerad/refs/heads/main/openapi/intelerad-openapi.yml
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
