---
api_key_in:
- header
api_specs:
- filename: tanium-platform-rest-api-openapi.yml
  format: yaml
  label: Tanium Platform REST API
  slug: platform-rest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tanium/refs/heads/main/openapi/tanium-platform-rest-api-openapi.yml
- filename: tanium-threat-response-api-openapi.yml
  format: yaml
  label: Tanium Threat Response API
  slug: threat-response-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tanium/refs/heads/main/openapi/tanium-threat-response-api-openapi.yml
- filename: tanium-connect-api-openapi.yml
  format: yaml
  label: Tanium Connect API
  slug: connect-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tanium/refs/heads/main/openapi/tanium-connect-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Tanium Authentication
name_suffix: Authentication
oauth_flows: []
overview: Tanium secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Tanium
provider_slug: tanium
scheme_count: 1
schemes:
- description: API token passed in the session header for authenticating with the Tanium Connect API.
  in: header
  name: apiToken
  parameter: session
  sources:
  - openapi/tanium-connect-api-openapi.yml
  - openapi/tanium-platform-rest-api-openapi.yml
  - openapi/tanium-threat-response-api-openapi.yml
  type: apiKey
slug: tanium-authentication
source_filename: tanium-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/tanium-connect-api-openapi.yml, openapi/tanium-platform-rest-api-openapi.yml,\n  openapi/tanium-threat-response-api-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: apiToken\n  type: apiKey\n  in: header\n  parameter: session\n  description: API token passed in the session header for authenticating with the Tanium Connect\n    API.\n  sources:\n  - openapi/tanium-connect-api-openapi.yml\n  - openapi/tanium-platform-rest-api-openapi.yml\n  - openapi/tanium-threat-response-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/tanium/refs/heads/main/authentication/tanium-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Compliance
- Endpoint Management
- Patch Management
- Security
- Threat Detection
- Unified Endpoint Management
---
