---
api_key_in:
- header
api_specs:
- filename: uplead-openapi.json
  format: json
  label: UpLead API
  slug: uplead-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/uplead/refs/heads/main/openapi/uplead-openapi.json
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Uplead Authentication
name_suffix: Authentication
oauth_flows: []
overview: UpLead secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: UpLead
provider_slug: uplead
scheme_count: 1
schemes:
- description: Your UpLead API key passed as a header value.
  in: header
  name: ApiKeyAuth
  parameter: Authorization
  sources:
  - openapi/uplead-openapi.json
  type: apiKey
slug: uplead-authentication
source_filename: uplead-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/uplead-openapi.json\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: ApiKeyAuth\n  type: apiKey\n  in: header\n  parameter: Authorization\n  description: Your UpLead API key passed as a header value.\n  sources:\n  - openapi/uplead-openapi.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/uplead/refs/heads/main/authentication/uplead-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- B2B
- Lead Generation
- Contact Data
- Company Data
- Email Verification
- Data Enrichment
- Sales Intelligence
---
