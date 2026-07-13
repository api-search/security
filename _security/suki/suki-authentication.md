---
api_key_in:
- header
api_specs:
- filename: suki-ambient-api-openapi.yml
  format: yaml
  label: Suki Ambient API
  slug: suki-ambient-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/suki/refs/heads/main/openapi/suki-ambient-api-openapi.yml
- filename: suki-dictation-api-openapi.yml
  format: yaml
  label: Suki Dictation API
  slug: suki-dictation-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/suki/refs/heads/main/openapi/suki-dictation-api-openapi.yml
- filename: suki-form-filling-api-openapi.yml
  format: yaml
  label: Suki Form Filling API
  slug: suki-form-filling-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/suki/refs/heads/main/openapi/suki-form-filling-api-openapi.yml
- filename: suki-auth-api-openapi.yml
  format: yaml
  label: Suki Auth API
  slug: suki-auth-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/suki/refs/heads/main/openapi/suki-auth-api-openapi.yml
- filename: suki-info-api-openapi.yml
  format: yaml
  label: Suki Info API
  slug: suki-info-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/suki/refs/heads/main/openapi/suki-info-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Suki Authentication
name_suffix: Authentication
oauth_flows: []
overview: Suki AI secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Suki AI
provider_slug: suki
scheme_count: 1
schemes:
- in: header
  name: SdpSukiToken
  parameter: sdp_suki_token
  sources:
  - openapi/suki-ambient-api-openapi.yml
  - openapi/suki-dictation-api-openapi.yml
  - openapi/suki-form-filling-api-openapi.yml
  - openapi/suki-info-api-openapi.yml
  type: apiKey
slug: suki-authentication
source_filename: suki-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/suki-ambient-api-openapi.yml, openapi/suki-dictation-api-openapi.yml, openapi/suki-form-filling-api-openapi.yml,\n  openapi/suki-info-api-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: SdpSukiToken\n  type: apiKey\n  in: header\n  parameter: sdp_suki_token\n  sources:\n  - openapi/suki-ambient-api-openapi.yml\n  - openapi/suki-dictation-api-openapi.yml\n  - openapi/suki-form-filling-api-openapi.yml\n  - openapi/suki-info-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/suki/refs/heads/main/authentication/suki-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- AI
- Artificial Intelligence
- Ambient Clinical Intelligence
- Medical Scribe
- Clinical Documentation
- Voice AI
- Speech Recognition
- Healthcare
- EHR Integration
- Epic
- Oracle Health
- athenahealth
- MEDITECH
- Dictation
- Form Filling
- Note Generation
- Generative AI
- HIPAA
- SOC2
- Healthcare Technology
---
