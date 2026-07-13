---
api_key_in:
- query
api_specs:
- filename: dns-check-openapi.yml
  format: yaml
  label: DNS Check REST API
  slug: rest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dns-check/refs/heads/main/openapi/dns-check-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Dns Check Authentication
name_suffix: Authentication
oauth_flows: []
overview: DNS Check secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: DNS Check
provider_slug: dns-check
scheme_count: 1
schemes:
- in: query
  name: apiKey
  parameter: api_key
  sources:
  - openapi/dns-check-openapi.yml
  type: apiKey
slug: dns-check-authentication
source_filename: dns-check-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/dns-check-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - query\nschemes:\n- name: apiKey\n  type: apiKey\n  in: query\n  parameter: api_key\n  sources:\n  - openapi/dns-check-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/dns-check/refs/heads/main/authentication/dns-check-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- DNS
- DNS Monitoring
- Domain Monitoring
- DNS Records
- Infrastructure Monitoring
- Networking
---
