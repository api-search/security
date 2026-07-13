---
api_key_in:
- header
api_specs:
- filename: ubiquiti-unifi-site-manager-api-openapi.yml
  format: yaml
  label: UniFi Site Manager API
  slug: unifi-site-manager-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ubiquiti/refs/heads/main/openapi/ubiquiti-unifi-site-manager-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Ubiquiti Authentication
name_suffix: Authentication
oauth_flows: []
overview: Ubiquiti secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Ubiquiti
provider_slug: ubiquiti
scheme_count: 1
schemes:
- description: API key generated at https://unifi.ui.com/settings/api-keys
  in: header
  name: ApiKeyAuth
  parameter: X-API-KEY
  sources:
  - openapi/ubiquiti-unifi-site-manager-api-openapi.yml
  type: apiKey
slug: ubiquiti-authentication
source_filename: ubiquiti-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/ubiquiti-unifi-site-manager-api-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: ApiKeyAuth\n  type: apiKey\n  in: header\n  parameter: X-API-KEY\n  description: API key generated at https://unifi.ui.com/settings/api-keys\n  sources:\n  - openapi/ubiquiti-unifi-site-manager-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/ubiquiti/refs/heads/main/authentication/ubiquiti-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Networking
- WiFi
- Switching
- Routing
- Surveillance
- Access Control
- ISP
- WISP
- UniFi
- UISP
- AmpliFi
---
