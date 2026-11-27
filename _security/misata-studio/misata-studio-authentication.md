---
anonymous_access: false
api_key_in: []
api_specs:
- filename: misata-studio-datasets-api-openapi.yml
  format: yaml
  label: Misata Datasets API
  slug: misata-studio-datasets-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/misata-studio/openapi/misata-studio-datasets-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: derived
name: Misata Authentication
name_suffix: Authentication
oauth_flows: []
overview: Misata secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Misata
provider_slug: misata-studio
scheme_count: 1
schemes:
- description: 'A Misata key, `Authorization: Bearer msk_...`: made in Studio, under API. A key is full or read (it reaches only the operations whose `x-misata-scope` is read), may have a monthly credit cap, and may expire'
  name: MisataKey
  scheme: bearer
  sources:
  - openapi/misata-studio-openapi.json
  type: http
slug: misata-studio-authentication
source_filename: misata-studio-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-18'\nmethod: derived\nsource: openapi/misata-studio-openapi.json\nsummary:\n  types:\n  - http\nschemes:\n- name: MisataKey\n  type: http\n  scheme: bearer\n  description: 'A Misata key, `Authorization: Bearer msk_...`: made in Studio, under API. A\n    key is full or read (it reaches only the operations whose `x-misata-scope` is read), may\n    have a monthly credit cap, and may expire'\n  sources:\n  - openapi/misata-studio-openapi.json\n"
source_yaml_url: https://artifacts.apis.io/misata-studio/authentication/misata-studio-authentication.yml
summary_line: http · 1 scheme
tags:
- Synthetic Data
- Artificial Intelligence
- Analytics
- Datasets
- Software-as-a-Service
---
