---
api_key_in:
- header
api_specs:
- filename: domains-openapi-original.yml
  format: yaml
  label: Gandi Domain API
  slug: domains
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gandi/refs/heads/main/openapi/domains-openapi-original.yml
- filename: livedns-openapi-original.yml
  format: yaml
  label: Gandi LiveDNS API
  slug: livedns
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gandi/refs/heads/main/openapi/livedns-openapi-original.yml
auth_types:
- apiKey
- http
description: ''
kind: authentication
layout: security
method: derived
name: Gandi Authentication
name_suffix: Authentication
oauth_flows: []
overview: Gandi secures its APIs with apiKey and http across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Gandi
provider_slug: gandi
scheme_count: 2
schemes:
- description: Personal Access Token (PAT) - format `Bearer pat_xxx`.
  name: bearer
  scheme: bearer
  sources:
  - openapi/domains-openapi-original.yml
  type: http
- description: Deprecated API key - format `Apikey YOUR_API_KEY`.
  in: header
  name: apiKey
  parameter: Authorization
  sources:
  - openapi/domains-openapi-original.yml
  - openapi/livedns-openapi-original.yml
  type: apiKey
slug: gandi-authentication
source_filename: gandi-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/domains-openapi-original.yml, openapi/livedns-openapi-original.yml\nsummary:\n  types:\n  - apiKey\n  - http\n  api_key_in:\n  - header\nschemes:\n- name: bearer\n  type: http\n  scheme: bearer\n  description: Personal Access Token (PAT) - format `Bearer pat_xxx`.\n  sources:\n  - openapi/domains-openapi-original.yml\n- name: apiKey\n  type: apiKey\n  in: header\n  parameter: Authorization\n  description: Deprecated API key - format `Apikey YOUR_API_KEY`.\n  sources:\n  - openapi/domains-openapi-original.yml\n  - openapi/livedns-openapi-original.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/gandi/refs/heads/main/authentication/gandi-authentication.yml
summary_line: apiKey/http · 2 schemes
tags:
- DNS
- Domains
- Domain Registrar
- Email
- Hosting
- Certificates
---
