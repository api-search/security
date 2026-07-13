---
api_key_in:
- header
api_specs:
- filename: openapi.yaml
  format: yaml
  label: Treasure Data TD API
  slug: treasure-data-td-api
  spec_type: OpenAPI
  url: https://api-docs.treasuredata.com/
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Treasure Data Authentication
name_suffix: Authentication
oauth_flows: []
overview: Treasure Data secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Treasure Data
provider_slug: treasure-data
scheme_count: 1
schemes:
- description: Treasure Data API key authentication. Set header value to "TD1 <your-api-key>".
  in: header
  name: TDAuth
  parameter: Authorization
  sources:
  - openapi/treasure-data-td-api-openapi.yml
  type: apiKey
slug: treasure-data-authentication
source_filename: treasure-data-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/treasure-data-td-api-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: TDAuth\n  type: apiKey\n  in: header\n  parameter: Authorization\n  description: Treasure Data API key authentication. Set header value to \"TD1 <your-api-key>\".\n  sources:\n  - openapi/treasure-data-td-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/treasure-data/refs/heads/main/authentication/treasure-data-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Customer Data Platform
- CDP
- Big Data
- Data Warehouse
- Hive
- Presto
- Enterprise
- AI
- Marketing
- Analytics
---
