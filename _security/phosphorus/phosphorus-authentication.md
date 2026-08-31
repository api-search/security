---
api_key_in:
- header
api_specs:
- filename: phosphorus-alerts-api-openapi.yml
  format: yaml
  label: Phosphorus Alerts API
  slug: phosphorus-alerts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/phosphorus/refs/heads/main/openapi/phosphorus-alerts-api-openapi.yml
- filename: phosphorus-device-api-openapi.yml
  format: yaml
  label: Phosphorus Device API
  slug: phosphorus-device-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/phosphorus/refs/heads/main/openapi/phosphorus-device-api-openapi.yml
- filename: phosphorus-devices-api-openapi.yml
  format: yaml
  label: Phosphorus Devices API
  slug: phosphorus-devices-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/phosphorus/refs/heads/main/openapi/phosphorus-devices-api-openapi.yml
- filename: phosphorus-dynamic-scans-api-openapi.yml
  format: yaml
  label: Phosphorus Dynamic Scans API
  slug: phosphorus-dynamic-scans-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/phosphorus/refs/heads/main/openapi/phosphorus-dynamic-scans-api-openapi.yml
- filename: phosphorus-providers-api-openapi.yml
  format: yaml
  label: Phosphorus Providers API
  slug: phosphorus-providers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/phosphorus/refs/heads/main/openapi/phosphorus-providers-api-openapi.yml
- filename: phosphorus-search-api-openapi.yml
  format: yaml
  label: Phosphorus Search API
  slug: phosphorus-search-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/phosphorus/refs/heads/main/openapi/phosphorus-search-api-openapi.yml
- filename: phosphorus-sites-api-openapi.yml
  format: yaml
  label: Phosphorus Sites API
  slug: phosphorus-sites-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/phosphorus/refs/heads/main/openapi/phosphorus-sites-api-openapi.yml
- filename: phosphorus-vault-api-openapi.yml
  format: yaml
  label: Phosphorus Vault API
  slug: phosphorus-vault-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/phosphorus/refs/heads/main/openapi/phosphorus-vault-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Phosphorus Authentication
name_suffix: Authentication
oauth_flows: []
overview: Phosphorus secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Phosphorus
provider_slug: phosphorus
scheme_count: 1
schemes:
- in: header
  name: ApiKeyAuth
  parameter: X-API-KEY
  sources:
  - openapi/phosphorus-api-openapi.yml
  type: apiKey
slug: phosphorus-authentication
source_filename: phosphorus-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-26'\nmethod: derived\nsource: openapi/phosphorus-api-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: ApiKeyAuth\n  type: apiKey\n  in: header\n  parameter: X-API-KEY\n  sources:\n  - openapi/phosphorus-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/phosphorus/refs/heads/main/authentication/phosphorus-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Cybersecurity
- xIoT Security
- IoT Security
- OT Security
- IoMT
- Asset Discovery
- Vulnerability Management
- Firmware Management
- Certificate Management
- Credential Management
- Critical Infrastructure
- Device Management
---
