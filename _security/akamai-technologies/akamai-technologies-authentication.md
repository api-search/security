---
api_key_in:
- header
api_specs:
- filename: akamai-technologies-openapi.yml
  format: yaml
  label: Akamai Technologies API
  slug: akamai-technologies-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/akamai-technologies/refs/heads/main/openapi/akamai-technologies-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Akamai Technologies Authentication
name_suffix: Authentication
oauth_flows: []
overview: Akamai Technologies secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Akamai Technologies
provider_slug: akamai-technologies
scheme_count: 1
schemes:
- description: 'Akamai EdgeGrid HMAC-SHA256 signed Authorization header

    (`EG1-HMAC-SHA256 client_token=...;access_token=...;timestamp=...;nonce=...;signature=...`).'
  in: header
  name: EdgeGrid
  parameter: Authorization
  sources:
  - openapi/akamai-technologies-openapi.yml
  type: apiKey
slug: akamai-technologies-authentication
source_filename: akamai-technologies-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/akamai-technologies-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: EdgeGrid\n  type: apiKey\n  in: header\n  parameter: Authorization\n  description: |-\n    Akamai EdgeGrid HMAC-SHA256 signed Authorization header\n    (`EG1-HMAC-SHA256 client_token=...;access_token=...;timestamp=...;nonce=...;signature=...`).\n  sources:\n  - openapi/akamai-technologies-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/akamai-technologies/refs/heads/main/authentication/akamai-technologies-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- CDN
- Security
- Cloud
---
