---
api_key_in:
- header
api_specs:
- filename: gandi-authorization-api-openapi.yml
  format: yaml
  label: Gandi Authorization API
  slug: gandi-authorization-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gandi/refs/heads/main/openapi/gandi-authorization-api-openapi.yml
- filename: gandi-availability-api-openapi.yml
  format: yaml
  label: Gandi Availability API
  slug: gandi-availability-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gandi/refs/heads/main/openapi/gandi-availability-api-openapi.yml
- filename: gandi-dnssec-api-openapi.yml
  format: yaml
  label: Gandi DNSSEC API
  slug: gandi-dnssec-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gandi/refs/heads/main/openapi/gandi-dnssec-api-openapi.yml
- filename: gandi-domains-api-openapi.yml
  format: yaml
  label: Gandi Domains API
  slug: gandi-domains-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gandi/refs/heads/main/openapi/gandi-domains-api-openapi.yml
- filename: gandi-ownership-api-openapi.yml
  format: yaml
  label: Gandi Ownership API
  slug: gandi-ownership-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gandi/refs/heads/main/openapi/gandi-ownership-api-openapi.yml
- filename: gandi-records-api-openapi.yml
  format: yaml
  label: Gandi Records API
  slug: gandi-records-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gandi/refs/heads/main/openapi/gandi-records-api-openapi.yml
- filename: gandi-renewal-api-openapi.yml
  format: yaml
  label: Gandi Renewal API
  slug: gandi-renewal-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gandi/refs/heads/main/openapi/gandi-renewal-api-openapi.yml
- filename: gandi-trademark-api-openapi.yml
  format: yaml
  label: Gandi Trademark API
  slug: gandi-trademark-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gandi/refs/heads/main/openapi/gandi-trademark-api-openapi.yml
- filename: gandi-tsig-api-openapi.yml
  format: yaml
  label: Gandi TSIG API
  slug: gandi-tsig-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gandi/refs/heads/main/openapi/gandi-tsig-api-openapi.yml
- filename: gandi-utilities-api-openapi.yml
  format: yaml
  label: Gandi Utilities API
  slug: gandi-utilities-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gandi/refs/heads/main/openapi/gandi-utilities-api-openapi.yml
- filename: gandi-zone-transfers-api-openapi.yml
  format: yaml
  label: Gandi Zone Transfers API
  slug: gandi-zone-transfers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gandi/refs/heads/main/openapi/gandi-zone-transfers-api-openapi.yml
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
- description: Personal Access Token (PAT) - format `Bearer [example key]`.
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
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/domains-openapi-original.yml, openapi/livedns-openapi-original.yml\nsummary:\n  types:\n  - apiKey\n  - http\n  api_key_in:\n  - header\nschemes:\n- name: bearer\n  type: http\n  scheme: bearer\n  description: Personal Access Token (PAT) - format `Bearer [example key]`.\n  sources:\n  - openapi/domains-openapi-original.yml\n- name: apiKey\n  type: apiKey\n  in: header\n  parameter: Authorization\n  description: Deprecated API key - format `Apikey YOUR_API_KEY`.\n  sources:\n  - openapi/domains-openapi-original.yml\n  - openapi/livedns-openapi-original.yml\n"
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
