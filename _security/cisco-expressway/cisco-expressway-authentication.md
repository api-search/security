---
api_key_in: []
api_specs:
- filename: cisco-expressway-configuration-api-openapi.yml
  format: yaml
  label: Cisco Expressway Configuration API
  slug: cisco-expressway-configuration-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cisco-expressway/refs/heads/main/openapi/cisco-expressway-configuration-api-openapi.yml
- filename: cisco-expressway-status-api-openapi.yml
  format: yaml
  label: Cisco Expressway Status API
  slug: cisco-expressway-status-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cisco-expressway/refs/heads/main/openapi/cisco-expressway-status-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Cisco Expressway Authentication
name_suffix: Authentication
oauth_flows: []
overview: Cisco Expressway secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Cisco Expressway
provider_slug: cisco-expressway
scheme_count: 1
schemes:
- description: HTTP Basic Authentication using Expressway administrator credentials. The API is only accessible via HTTPS.
  name: basicAuth
  scheme: basic
  sources:
  - openapi/cisco-expressway-configuration-api-openapi.yml
  - openapi/cisco-expressway-status-api-openapi.yml
  type: http
slug: cisco-expressway-authentication
source_filename: cisco-expressway-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/cisco-expressway-configuration-api-openapi.yml, openapi/cisco-expressway-status-api-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: basicAuth\n  type: http\n  scheme: basic\n  description: HTTP Basic Authentication using Expressway administrator credentials. The API\n    is only accessible via HTTPS.\n  sources:\n  - openapi/cisco-expressway-configuration-api-openapi.yml\n  - openapi/cisco-expressway-status-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/cisco-expressway/refs/heads/main/authentication/cisco-expressway-authentication.yml
summary_line: http · 1 scheme
tags:
- Collaboration
- Firewall Traversal
- H.323
- Session Border Controller
- SIP
- Unified Communications
- Video Conferencing
---
