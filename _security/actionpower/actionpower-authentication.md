---
anonymous_access: false
api_key_in: []
api_specs:
- filename: actionpower-daglo-cloud-api-openapi.yml
  format: yaml
  label: daglo Cloud API
  slug: daglo-cloud-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/actionpower/refs/heads/main/openapi/actionpower-daglo-cloud-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: derived
name: Actionpower Authentication
name_suffix: Authentication
oauth_flows: []
overview: Actionpower secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Actionpower
provider_slug: actionpower
scheme_count: 1
schemes:
- name: BearerAuth
  scheme: bearer
  sources:
  - openapi/actionpower-daglo-cloud-api-dev-openapi.yml
  - openapi/actionpower-daglo-cloud-api-openapi.yml
  type: http
slug: actionpower-authentication
source_filename: actionpower-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-09-06'\nmethod: derived\nsource: openapi/actionpower-daglo-cloud-api-dev-openapi.yml, openapi/actionpower-daglo-cloud-api-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: BearerAuth\n  type: http\n  scheme: bearer\n  sources:\n  - openapi/actionpower-daglo-cloud-api-dev-openapi.yml\n  - openapi/actionpower-daglo-cloud-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/actionpower/refs/heads/main/authentication/actionpower-authentication.yml
summary_line: http · 1 scheme
tags:
- Speech Recognition
- Speech To Text
- Text To Speech
- Natural Language Processing
- Artificial Intelligence
- Transcription
- Voice
- Meeting Intelligence
- gRPC
- South Korea
---
