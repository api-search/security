---
api_key_in:
- query
api_specs:
- filename: completedns-v2-openapi.yml
  format: yaml
  label: CompleteDNS API v2
  slug: dns-history-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/completedns/refs/heads/main/openapi/completedns-v2-openapi.yml
- filename: completedns-v1-openapi.yml
  format: yaml
  label: CompleteDNS API v1
  slug: ns-history-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/completedns/refs/heads/main/openapi/completedns-v1-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Completedns Authentication
name_suffix: Authentication
oauth_flows: []
overview: CompleteDNS secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: CompleteDNS
provider_slug: completedns
scheme_count: 1
schemes:
- in: query
  name: apiKey
  parameter: key
  sources:
  - openapi/completedns-v1-openapi.yml
  - openapi/completedns-v2-openapi.yml
  type: apiKey
slug: completedns-authentication
source_filename: completedns-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/completedns-v1-openapi.yml, openapi/completedns-v2-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - query\nschemes:\n- name: apiKey\n  type: apiKey\n  in: query\n  parameter: key\n  sources:\n  - openapi/completedns-v1-openapi.yml\n  - openapi/completedns-v2-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/completedns/refs/heads/main/authentication/completedns-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- DNS
- DNS History
- Domain Intelligence
- Domains
- Nameservers
- Threat Intelligence
---
