---
api_key_in:
- header
api_specs:
- filename: metriport-openapi.yml
  format: yaml
  label: Metriport Medical Patients API
  slug: medical-patients
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/metriport/refs/heads/main/openapi/metriport-openapi.yml
- filename: metriport-openapi.yml
  format: yaml
  label: Metriport Medical Facilities API
  slug: medical-facilities
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/metriport/refs/heads/main/openapi/metriport-openapi.yml
- filename: metriport-openapi.yml
  format: yaml
  label: Metriport Medical Document Query API
  slug: medical-document-query
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/metriport/refs/heads/main/openapi/metriport-openapi.yml
- filename: metriport-openapi.yml
  format: yaml
  label: Metriport Medical Consolidated FHIR API
  slug: medical-consolidated-fhir
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/metriport/refs/heads/main/openapi/metriport-openapi.yml
- filename: metriport-openapi.yml
  format: yaml
  label: Metriport Devices Users API
  slug: devices-users
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/metriport/refs/heads/main/openapi/metriport-openapi.yml
- filename: metriport-openapi.yml
  format: yaml
  label: Metriport Devices Biometrics API
  slug: devices-biometrics
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/metriport/refs/heads/main/openapi/metriport-openapi.yml
- filename: metriport-openapi.yml
  format: yaml
  label: Metriport Webhooks API
  slug: webhooks
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/metriport/refs/heads/main/openapi/metriport-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Metriport Authentication
name_suffix: Authentication
oauth_flows: []
overview: Metriport secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Metriport
provider_slug: metriport
scheme_count: 1
schemes:
- in: header
  name: ApiKeyAuth
  parameter: x-api-key
  sources:
  - openapi/metriport-openapi.yml
  type: apiKey
slug: metriport-authentication
source_filename: metriport-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/metriport-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: ApiKeyAuth\n  type: apiKey\n  in: header\n  parameter: x-api-key\n  sources:\n  - openapi/metriport-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/metriport/refs/heads/main/authentication/metriport-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Healthcare
- Medical Records
- FHIR
- Health Data
- Wearables
- Open Source
---
