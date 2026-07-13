---
api_key_in:
- header
api_specs:
- filename: openprovider-openapi.json
  format: json
  label: Openprovider API
  slug: openprovider-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/openprovider/refs/heads/main/openapi/openprovider-openapi.json
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Openprovider Authentication
name_suffix: Authentication
oauth_flows: []
overview: Openprovider secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Openprovider
provider_slug: openprovider
scheme_count: 1
schemes:
- in: header
  name: Bearer
  parameter: Authorization
  sources:
  - openapi/openprovider-openapi.json
  type: apiKey
slug: openprovider-authentication
source_filename: openprovider-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/openprovider-openapi.json\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: Bearer\n  type: apiKey\n  in: header\n  parameter: Authorization\n  sources:\n  - openapi/openprovider-openapi.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/openprovider/refs/heads/main/authentication/openprovider-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Domains
- DNS
- Hosting
- Reseller
- SSL Certificates
- TLDs
---
