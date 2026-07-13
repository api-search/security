---
api_key_in:
- query
api_specs:
- filename: parsehub-openapi.yml
  format: yaml
  label: ParseHub
  slug: parsehub
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/parsehub/refs/heads/main/openapi/parsehub-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Parsehub Authentication
name_suffix: Authentication
oauth_flows: []
overview: ParseHub secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: ParseHub
provider_slug: parsehub
scheme_count: 1
schemes:
- in: query
  name: apiKey
  parameter: api_key
  sources:
  - openapi/parsehub-openapi.yml
  type: apiKey
slug: parsehub-authentication
source_filename: parsehub-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/parsehub-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - query\nschemes:\n- name: apiKey\n  type: apiKey\n  in: query\n  parameter: api_key\n  sources:\n  - openapi/parsehub-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/parsehub/refs/heads/main/authentication/parsehub-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Data Extraction
- Scraping
- Visual Scraping
---
