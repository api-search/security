---
api_key_in: []
api_specs:
- filename: lex-machina-openapi.yml
  format: yaml
  label: Lex Machina Litigation Analytics API
  slug: lex-machina-litigation-analytics-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lex-machina/refs/heads/main/openapi/lex-machina-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Lex Machina Authentication
name_suffix: Authentication
oauth_flows: []
overview: Lex Machina secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Lex Machina
provider_slug: lex-machina
scheme_count: 1
schemes:
- name: JwtAccessBearer
  scheme: bearer
  sources:
  - openapi/lex-machina-openapi.yml
  type: http
slug: lex-machina-authentication
source_filename: lex-machina-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/lex-machina-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: JwtAccessBearer\n  type: http\n  scheme: bearer\n  sources:\n  - openapi/lex-machina-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/lex-machina/refs/heads/main/authentication/lex-machina-authentication.yml
summary_line: http · 1 scheme
tags:
- Legal
- Legal Analytics
- Legal Technology
- Litigation
- Litigation Analytics
- Court Data
- Dockets
- Judges
- Law Firms
- Attorneys
- Patents
- PTAB
- ITC
- Bankruptcy
- Appeals
- State Courts
- Federal Courts
- LexisNexis
- Data
- Analytics
---
