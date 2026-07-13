---
api_key_in:
- header
api_specs:
- filename: truphone-openapi.yml
  format: yaml
  label: Truphone (1GLOBAL) SIMs / eSIMs API
  slug: truphone-sims-esims-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/truphone/refs/heads/main/openapi/truphone-openapi.yml
- filename: truphone-openapi.yml
  format: yaml
  label: Truphone (1GLOBAL) Connectivity / Usage API
  slug: truphone-connectivity-usage-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/truphone/refs/heads/main/openapi/truphone-openapi.yml
- filename: truphone-openapi.yml
  format: yaml
  label: Truphone (1GLOBAL) Plans API
  slug: truphone-plans-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/truphone/refs/heads/main/openapi/truphone-openapi.yml
- filename: truphone-openapi.yml
  format: yaml
  label: Truphone (1GLOBAL) Device Management API
  slug: truphone-device-management-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/truphone/refs/heads/main/openapi/truphone-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Truphone Authentication
name_suffix: Authentication
oauth_flows: []
overview: Truphone (1GLOBAL) secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Truphone (1GLOBAL)
provider_slug: truphone
scheme_count: 1
schemes:
- description: 'Token-based authentication. Supply the header `Authorization: Token <api-key>`. (1GLOBAL Connect and the 1GLOBAL platform API on services.truphone.com use OAuth2 / bearer tokens instead; see provider documentation.)'
  in: header
  name: TokenAuth
  parameter: Authorization
  sources:
  - openapi/truphone-openapi.yml
  type: apiKey
slug: truphone-authentication
source_filename: truphone-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/truphone-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: TokenAuth\n  type: apiKey\n  in: header\n  parameter: Authorization\n  description: 'Token-based authentication. Supply the header `Authorization: Token <api-key>`.\n    (1GLOBAL Connect and the 1GLOBAL platform API on services.truphone.com use OAuth2 / bearer\n    tokens instead; see provider documentation.)'\n  sources:\n  - openapi/truphone-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/truphone/refs/heads/main/authentication/truphone-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- eSIM
- IoT
- Connectivity
- SIM Management
- Telecom
- Mobile Network
---
