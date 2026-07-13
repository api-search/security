---
api_key_in:
- header
api_specs:
- filename: abuseipdb-apiv2-openapi.yml
  format: yaml
  label: AbuseIPDB APIv2
  slug: apiv2
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/abuseipdb/refs/heads/main/openapi/abuseipdb-apiv2-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Abuseipdb Authentication
name_suffix: Authentication
oauth_flows: []
overview: AbuseIPDB secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: AbuseIPDB
provider_slug: abuseipdb
scheme_count: 1
schemes:
- description: AbuseIPDB API key. Issue and rotate at https://www.abuseipdb.com/account/api.
  in: header
  name: ApiKeyAuth
  parameter: Key
  sources:
  - openapi/abuseipdb-apiv2-openapi.yml
  type: apiKey
slug: abuseipdb-authentication
source_filename: abuseipdb-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/abuseipdb-apiv2-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: ApiKeyAuth\n  type: apiKey\n  in: header\n  parameter: Key\n  description: AbuseIPDB API key. Issue and rotate at https://www.abuseipdb.com/account/api.\n  sources:\n  - openapi/abuseipdb-apiv2-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/abuseipdb/refs/heads/main/authentication/abuseipdb-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Anti Malware
- Blacklist
- Cyber Security
- IP Reputation
- Network Security
- Public APIs
- Threat Intelligence
---
