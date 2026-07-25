---
api_key_in:
- header
api_specs:
- filename: metriport-consolidated-api-openapi.yml
  format: yaml
  label: Metriport Consolidated API
  slug: metriport-consolidated-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/metriport/refs/heads/main/openapi/metriport-consolidated-api-openapi.yml
- filename: metriport-devices-data-api-openapi.yml
  format: yaml
  label: Metriport Devices Data API
  slug: metriport-devices-data-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/metriport/refs/heads/main/openapi/metriport-devices-data-api-openapi.yml
- filename: metriport-document-api-openapi.yml
  format: yaml
  label: Metriport Document API
  slug: metriport-document-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/metriport/refs/heads/main/openapi/metriport-document-api-openapi.yml
- filename: metriport-facility-api-openapi.yml
  format: yaml
  label: Metriport Facility API
  slug: metriport-facility-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/metriport/refs/heads/main/openapi/metriport-facility-api-openapi.yml
- filename: metriport-patient-api-openapi.yml
  format: yaml
  label: Metriport Patient API
  slug: metriport-patient-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/metriport/refs/heads/main/openapi/metriport-patient-api-openapi.yml
- filename: metriport-settings-api-openapi.yml
  format: yaml
  label: Metriport Settings API
  slug: metriport-settings-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/metriport/refs/heads/main/openapi/metriport-settings-api-openapi.yml
- filename: metriport-user-api-openapi.yml
  format: yaml
  label: Metriport User API
  slug: metriport-user-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/metriport/refs/heads/main/openapi/metriport-user-api-openapi.yml
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
