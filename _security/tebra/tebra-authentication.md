---
api_key_in:
- header
api_specs:
- filename: tebra-clinical-openapi.yml
  format: yaml
  label: Tebra Clinical Data API
  slug: tebra-clinical-data-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tebra/refs/heads/main/openapi/tebra-clinical-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Tebra Authentication
name_suffix: Authentication
oauth_flows: []
overview: Tebra secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Tebra
provider_slug: tebra
scheme_count: 1
schemes:
- description: Patient-generated API Key from the Tebra Patient Portal (My Account > API Access Key). A missing, revoked, or invalid key returns 401 Unauthorized.
  in: header
  name: apiKeyAuth
  parameter: X-Api-Key
  sources:
  - openapi/tebra-clinical-openapi.yml
  type: apiKey
slug: tebra-authentication
source_filename: tebra-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/tebra-clinical-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: apiKeyAuth\n  type: apiKey\n  in: header\n  parameter: X-Api-Key\n  description: Patient-generated API Key from the Tebra Patient Portal (My Account > API Access\n    Key). A missing, revoked, or invalid key returns 401 Unauthorized.\n  sources:\n  - openapi/tebra-clinical-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/tebra/refs/heads/main/authentication/tebra-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Healthcare
- Practice Management
- EHR
- Medical Billing
- Patient Engagement
- Kareo
- PatientPop
---
