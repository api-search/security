---
api_key_in:
- header
api_specs:
- filename: cyble-odin-openapi.yml
  format: yaml
  label: ODIN API
  slug: odin-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cyble/refs/heads/main/openapi/cyble-odin-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Cyble Authentication
name_suffix: Authentication
oauth_flows: []
overview: Cyble secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Cyble
provider_slug: cyble
scheme_count: 1
schemes:
- in: header
  name: ApiKeyAuth
  parameter: X-API-Key
  sources:
  - openapi/cyble-odin-openapi.yml
  type: apiKey
slug: cyble-authentication
source_filename: cyble-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-11'\nmethod: derived\nsource: openapi/cyble-odin-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: ApiKeyAuth\n  type: apiKey\n  in: header\n  parameter: X-API-Key\n  sources:\n  - openapi/cyble-odin-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/cyble/refs/heads/main/authentication/cyble-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Threat Intelligence
- Cybersecurity
- Attack Surface Management
- Internet Scanning
- Dark Web Monitoring
- Vulnerability Management
- CVE
- exposed-buckets
- Domain Intelligence
- WHOIS
- OSINT
- Security
---
