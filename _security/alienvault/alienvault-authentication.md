---
api_key_in:
- header
api_specs:
- filename: alienvault-otx-openapi.yml
  format: yaml
  label: AlienVault OTX DirectConnect API
  slug: alienvault-otx-directconnect-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/alienvault/refs/heads/main/openapi/alienvault-otx-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: searched
name: Alienvault Authentication
name_suffix: Authentication
oauth_flows: []
overview: AlienVault secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: AlienVault
provider_slug: alienvault
scheme_count: 1
schemes:
- description: OTX API key, available from your OTX account settings page.
  in: header
  name: OTXApiKey
  parameter: X-OTX-API-KEY
  sources:
  - openapi/alienvault-otx-openapi.yml
  type: apiKey
slug: alienvault-authentication
source_filename: alienvault-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-17'\nmethod: searched\nsource: openapi/alienvault-otx-openapi.yml\ndocs: https://otx.alienvault.com/api\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: OTXApiKey\n  type: apiKey\n  in: header\n  parameter: X-OTX-API-KEY\n  description: OTX API key, available from your OTX account settings page.\n  sources:\n  - openapi/alienvault-otx-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/alienvault/refs/heads/main/authentication/alienvault-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Company
- Security
- Threat Intelligence
- Cybersecurity
- Open Threat Exchange
- Indicators of Compromise
- Threat Feeds
- API
---
